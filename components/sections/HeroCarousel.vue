<template>
  <div class="flex items-center justify-center h-full">
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
        class="w-full max-w-[280px] sm:max-w-[400px] md:max-w-[500px] lg:max-w-[600px] rounded-full overflow-hidden"
      >
        <swiper-slide v-for="(image, index) in images" :key="index">
          <div class="relative aspect-square rounded-full overflow-hidden">
            <img
              :src="image"
              :alt="`Restaurante ${index + 1}`"
              class="w-full h-full object-cover"
            />
          </div>
        </swiper-slide>
      </swiper-container>
    </ClientOnly>
  </div>
</template>

<script setup>
const containerRef = ref(null);
const images = ["/customers/restaurant-1.png", "/customers/restaurant-2.png"];

const swiper = useSwiper(containerRef, {
  modules: ["autoplay"],
  autoplay: {
    delay: 3000,
    disableOnInteraction: false,
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
