<template>
  <section class="py-20 bg-gradient-to-b from-muted to-background">
    <div class="container mx-auto px-4">
      <div class="max-w-4xl mx-auto text-center mb-12">
        <h2
          class="text-4xl font-bold mb-6 bg-gradient-to-r from-primary to-primary/80 bg-clip-text text-transparent"
        >
          Nossos Clientes em Ação
        </h2>
        <p class="text-lg text-muted-foreground">
          Veja como nossos clientes estão transformando a experiência dos seus
          restaurantes com nossa solução
        </p>
      </div>

      <div class="max-w-5xl mx-auto">
        <ClientOnly>
          <swiper-container
            ref="containerRef"
            :slides-per-view="1"
            :space-between="30"
            :loop="true"
            :autoplay="{
              delay: 3000,
              disableOnInteraction: false,
            }"
            class="w-full rounded-xl overflow-hidden"
          >
            <swiper-slide v-for="(image, index) in images" :key="index">
              <div class="relative aspect-[16/9] rounded-xl overflow-hidden">
                <img
                  :src="image"
                  :alt="`Implementação ${index + 1}`"
                  class="w-full h-full object-cover"
                />
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
const images = [
  "/real-customers/image-1.jpg",
  "/real-customers/image-2.png",
  "/real-customers/image-3.png",
  "/real-customers/image-4.png",
];

const swiper = useSwiper(containerRef, {
  modules: ["autoplay", "pagination"],
  autoplay: {
    delay: 3000,
    disableOnInteraction: true,
  },
  loop: true,
  slidesPerView: 1,
  spaceBetween: 30,
});
</script>

<style scoped>
swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
