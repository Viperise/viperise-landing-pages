<template>
  <section class="py-20 bg-gradient-to-b from-muted to-background">
    <div class="container mx-auto px-4">
      <div class="max-w-4xl mx-auto text-center mb-12">
        <h2
          class="text-4xl font-bold mb-6 bg-gradient-to-r from-primary to-primary/80 bg-clip-text text-transparent"
        >
          Cardápio Digital + Anúncios de Alta Conversão
        </h2>
        <p class="text-lg text-muted-foreground">
          Veja como nossos clientes estão aumentando suas vendas com cardápios
          digitais interativos e anúncios personalizados que convertem
        </p>
      </div>

      <div class="max-w-5xl mx-auto relative">
        <ClientOnly>
          <swiper-container
            ref="containerRef"
            :slides-per-view="1"
            :space-between="30"
            :loop="true"
            :pagination="{
              clickable: true,
              dynamicBullets: true,
            }"
            :navigation="true"
            :autoplay="{
              delay: 5000,
              disableOnInteraction: false,
              pauseOnMouseEnter: true,
            }"
            class="w-full rounded-xl overflow-hidden"
          >
            <swiper-slide v-for="(video, index) in videos" :key="index">
              <div
                class="relative w-full md:w-[80%] mx-auto aspect-video rounded-xl overflow-hidden bg-black"
              >
                <video
                  :src="video"
                  class="absolute inset-0 w-full h-full object-cover"
                  controls
                  preload="metadata"
                  @play="handleVideoPlay"
                  @pause="handleVideoPause"
                  @ended="handleVideoEnded"
                >
                  Seu navegador não suporta o elemento de vídeo.
                </video>
              </div>
            </swiper-slide>
          </swiper-container>
        </ClientOnly>
      </div>
    </div>
  </section>
</template>

<script setup>
const containerRef = ref(null);
const videos = [
  "/real-customers/videos/video-1.mp4",
  "/real-customers/videos/video-2.mp4",
  "/real-customers/videos/video-3.mp4",
  "/real-customers/videos/video-4.mp4",
  "/real-customers/videos/video-5.mp4",
  "/real-customers/videos/video-6.mp4",
  "/real-customers/videos/video-7.mp4",
];

const swiper = useSwiper(containerRef, {
  modules: ["autoplay", "pagination", "navigation"],
  autoplay: {
    delay: 5000,
    disableOnInteraction: false,
  },
  pagination: {
    clickable: true,
    dynamicBullets: true,
  },
  navigation: true,
  loop: true,
  slidesPerView: 1,
  spaceBetween: 30,
});

const handleVideoPlay = () => {
  swiper.value?.autoplay?.stop();
};

const handleVideoPause = () => {
  swiper.value?.autoplay?.start();
};

const handleVideoEnded = () => {
  swiper.value?.autoplay?.start();
};
</script>

<style scoped>
swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

:deep(.swiper-pagination-bullet) {
  background-color: #ffbb00 !important;
  opacity: 0.5 !important;
}

:deep(.swiper-pagination-bullet-active) {
  opacity: 1 !important;
  background-color: #ffbb00 !important;
}

:deep(.swiper-button-next),
:deep(.swiper-button-prev) {
  color: #ffbb00 !important;
  background: rgba(0, 0, 0, 0.3);
  width: 40px;
  height: 40px;
  border-radius: 50%;
  transition: background-color 0.3s;
}

:deep(.swiper-button-next:hover),
:deep(.swiper-button-prev:hover) {
  background: rgba(0, 0, 0, 0.5);
}

:deep(.swiper-button-next::after),
:deep(.swiper-button-prev::after) {
  font-size: 20px;
  color: #ffbb00 !important;
}

@media (max-width: 768px) {
  .swiper-slide > div {
    width: 100% !important;
  }
}
</style>
