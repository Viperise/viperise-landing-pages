<template>
  <div class="min-h-screen bg-white text-gray-900">
    <!-- Header -->
    <Header />

    <!-- Hero Section -->
    <HeroSection />

    <!-- Services Section -->
    <ServicesSection />

    <!-- About Section -->
    <AboutSection />

    <!-- Contact Section -->
    <ContactSection />

    <!-- Footer -->
    <Footer />
  </div>
</template>

<script setup>
import { Header, Footer } from "@/components/layout";
import {
  HeroSection,
  ServicesSection,
  AboutSection,
  ContactSection,
} from "@/components/sections";
</script>

<style scoped>
/* Custom scrollbar for webkit browsers */
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: #f3f4f6;
}

::-webkit-scrollbar-thumb {
  background: #dc2626;
  border-radius: 4px;
}

::-webkit-scrollbar-thumb:hover {
  background: #b91c1c;
}

/* Smooth transitions */
* {
  transition: all 0.3s ease;
}

/* Gradient text animation */
@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

.bg-gradient-to-r {
  background-size: 200% 200%;
  animation: gradient 3s ease infinite;
}
</style>
