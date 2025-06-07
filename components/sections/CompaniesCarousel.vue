<template>
  <div class="w-full bg-gray-900 py-12 overflow-hidden">
    <div class="container mx-auto px-4 mb-8 text-center">
      <h2 class="text-3xl font-bold text-white mb-4">
        Empresas que já confiam no Reachout
      </h2>
      <p class="text-lg text-gray-300 max-w-2xl mx-auto">
        Conheça algumas das empresas que já utilizaram nossa plataforma para
        alcançar seus objetivos de marketing digital
      </p>
    </div>
    <div class="relative w-full overflow-hidden">
      <div class="flex animate-scroll space-x-8">
        <!-- Primeiro conjunto de logos -->
        <div
          v-for="(company, index) in companies"
          :key="index"
          class="flex-shrink-0"
        >
          <img
            :src="`/companies/${company.image}`"
            :alt="company.name"
            class="h-16 object-contain"
          />
        </div>
        <!-- Segundo conjunto de logos (para o efeito infinito) -->
        <div
          v-for="(company, index) in companies"
          :key="'duplicate-' + index"
          class="flex-shrink-0"
        >
          <img
            :src="`/companies/${company.image}`"
            :alt="company.name"
            class="h-16 object-contain"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const companies = [
  { name: "Performe", image: "performe.jpg" },
  { name: "Equilíbrio", image: "equilibrio.png" },
  { name: "Betel Kids", image: "betel-kids.jpg" },
  { name: "Monte Carlo", image: "monte-carlo.png" },
  { name: "Brenda Silva Boutique", image: "brenda-silva-boutique.png" },
  { name: "Imunoclin", image: "imunoclin.webp" },
  { name: "Silva Car", image: "silva-car.jpg" },
  { name: "Valle", image: "valle.svg" },
];
</script>

<style scoped>
.animate-scroll {
  animation: scroll 30s linear infinite forwards;
}

@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-100%);
  }
}
</style>
