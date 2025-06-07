<template>
  <section class="py-8 bg-muted/50">
    <div class="w-full overflow-hidden">
      <ClientOnly>
        <swiper-container
          ref="containerRef"
          :slides-per-view="'auto'"
          :space-between="30"
          :loop="true"
          :autoplay="{
            delay: 0,
            disableOnInteraction: false,
          }"
          :speed="5000"
          class="w-full"
        >
          <swiper-slide
            v-for="(company, index) in companies"
            :key="index"
            class="!w-auto"
          >
            <div class="h-16 flex items-center justify-center px-4">
              <img
                :src="company"
                :alt="`Logo da empresa ${index + 1}`"
                class="h-full w-auto object-contain grayscale hover:grayscale-0 transition-all duration-300"
              />
            </div>
          </swiper-slide>
        </swiper-container>
      </ClientOnly>
    </div>
  </section>
</template>

<script setup>
const containerRef = ref(null);

const companies = [
  "/companies/performe.jpg",
  "/companies/equilibrio.png",
  "/companies/betel-kids.jpg",
  "/companies/monte-carlo.png",
  "/companies/brenda-silva-boutique.png",
  "/companies/imunoclin.webp",
  "/companies/silva-car.jpg",
  "/companies/valle.svg",
];

const swiper = useSwiper(containerRef, {
  modules: ["autoplay"],
  autoplay: {
    delay: 0,
    disableOnInteraction: false,
  },
  loop: true,
  slidesPerView: "auto",
  spaceBetween: 30,
  speed: 5000,
});
</script>

<style scoped>
swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 64px;
}

img {
  max-height: 100%;
  width: auto;
  filter: grayscale(100%);
  transition: filter 0.3s ease;
}

img:hover {
  filter: grayscale(0%);
}
</style>
