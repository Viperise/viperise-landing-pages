<template>
  <div class="min-h-screen bg-background">
    <Header />
    <HeroSection />
    <AdPotentialSection />
    <RealCustomersGallery />
    <SystemVideosSection />
    <CompaniesCarousel />
    <PricingSection />
  </div>
</template>

<script setup>
import Header from "@/components/layout/Header.vue";
import HeroSection from "@/components/sections/HeroSection.vue";
import AdPotentialSection from "@/components/sections/AdPotentialSection.vue";
import SystemVideosSection from "@/components/sections/SystemVideosSection.vue";
import RealCustomersGallery from "@/components/sections/RealCustomersGallery.vue";
import CompaniesCarousel from "@/components/sections/CompaniesCarousel.vue";
import PricingSection from "@/components/sections/PricingSection.vue";

useSeoMeta({
  title: "Reachout - Plataforma de Anúncios e Vendas",
  meta: [
    {
      name: "description",
      content:
        "Reachout: A plataforma definitiva para criar e gerenciar anúncios de vendas. Aumente suas vendas com nossa solução completa de marketing digital e automação de anúncios.",
    },
    {
      name: "keywords",
      content:
        "anúncios de venda, marketing digital, automação de anúncios, plataforma de vendas, gestão de anúncios, marketing online, vendas online",
    },
    { name: "author", content: "daywison silva, viperise" },
    { name: "robots", content: "index, follow" },
  ],
  ogImage: "https://i.ibb.co/hJdyMsNb/og-image.png",
  ogImageSecureUrl: "https://i.ibb.co/hJdyMsNb/og-image.png",
  ogImageType: "image/png",
  ogImageWidth: 493,
  ogImageHeight: 259,
  ogImageAlt: "Reachout - Plataforma de Anúncios e Vendas",
  twitterImage: "/og-image.png",
  twitterCard: "summary_large_image",
  twitterTitle: "Reachout - Plataforma de Anúncios e Vendas",
  twitterDescription:
    "Reachout: A plataforma definitiva para criar e gerenciar anúncios de vendas. Aumente suas vendas com nossa solução completa de marketing digital e automação de anúncios.",
  twitterSite: "@reachout",
  twitterCreator: "@reachout",
});
</script>
