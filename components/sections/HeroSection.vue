<template>
  <section class="pt-24 pb-12 md:pt-32 md:pb-16 lg:pt-40 lg:pb-24">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid gap-8 md:gap-12 lg:grid-cols-2 lg:gap-16 items-center">
        <div class="order-2 lg:order-1">
          <HeroContent />
        </div>
        <div class="order-1 lg:order-2">
          <HeroCarousel />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import HeroContent from "./HeroContent.vue";
import HeroCarousel from "./HeroCarousel.vue";
</script>

<style>
swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-pagination-bullet {
  background: #000 !important;
  opacity: 0.5;
}

.swiper-pagination-bullet-active {
  opacity: 1 !important;
}
</style>
