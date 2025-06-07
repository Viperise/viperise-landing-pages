<template>
  <div class="min-h-screen bg-background">
    <Header />
    <HeroSection />
    <AdPotentialSection />
    <RealCustomersGallery />
    <SystemVideosSection />
    <CompaniesCarousel />
  </div>
</template>

<script setup>
import Header from "@/components/layout/Header.vue";
import HeroSection from "@/components/sections/HeroSection.vue";
import AdPotentialSection from "@/components/sections/AdPotentialSection.vue";
import SystemVideosSection from "@/components/sections/SystemVideosSection.vue";
import RealCustomersGallery from "@/components/sections/RealCustomersGallery.vue";
import CompaniesCarousel from "@/components/sections/CompaniesCarousel.vue";
</script>
