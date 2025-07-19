<template>
  <section id="home" class="pt-24 pb-16 px-4 relative overflow-hidden">
    <!-- Background Pattern -->
    <div
      class="absolute inset-0 bg-gradient-to-br from-red-50 via-white to-red-100"
    ></div>

    <!-- Animated Background Elements -->
    <div class="absolute inset-0">
      <div
        class="absolute top-20 left-10 w-32 h-32 bg-red-200 rounded-full opacity-20 animate-float"
      ></div>
      <div
        class="absolute top-40 right-20 w-24 h-24 bg-red-300 rounded-full opacity-15 animate-float-slow"
      ></div>
      <div
        class="absolute bottom-20 left-1/4 w-16 h-16 bg-red-400 rounded-full opacity-25 animate-float"
      ></div>
      <div
        class="absolute bottom-40 right-1/3 w-20 h-20 bg-red-200 rounded-full opacity-20 animate-float-slow"
      ></div>
    </div>

    <!-- Geometric Shapes -->
    <div class="absolute inset-0">
      <div
        class="absolute top-32 left-1/3 w-8 h-8 bg-red-300 transform rotate-45 opacity-30 animate-float-slow"
      ></div>
      <div
        class="absolute bottom-32 right-1/4 w-12 h-12 bg-red-400 transform rotate-12 opacity-25 animate-float"
      ></div>
      <div
        class="absolute top-1/2 left-20 w-6 h-6 bg-red-500 transform rotate-45 opacity-20 animate-float-slow"
      ></div>
      <div
        class="absolute top-1/3 right-10 w-10 h-10 bg-red-200 transform rotate-30 opacity-25 animate-float"
      ></div>
      <div
        class="absolute bottom-1/3 left-1/2 w-4 h-4 bg-red-300 transform rotate-60 opacity-30 animate-float-slow"
      ></div>
    </div>

    <!-- Subtle Grid Pattern -->
    <div class="absolute inset-0 opacity-5">
      <div
        class="absolute inset-0"
        style="
          background-image: radial-gradient(
            circle at 1px 1px,
            rgba(220, 38, 38, 0.3) 1px,
            transparent 0
          );
          background-size: 50px 50px;
        "
      ></div>
    </div>

    <!-- Content Container -->
    <div class="relative z-10">
      <div class="container mx-auto text-center">
        <div class="max-w-4xl mx-auto">
          <Badge
            variant="secondary"
            class="mb-6 bg-red-100 text-red-700 border-red-200"
          >
            Software House de Excelência
          </Badge>
          <h1
            class="text-5xl md:text-7xl font-bold mb-6 bg-gradient-to-r from-red-600 via-red-700 to-red-800 bg-clip-text text-transparent"
          >
            Transformamos Ideias em
            <span class="block leading-16 md:leading-24"
              >Realidade Digital</span
            >
          </h1>
          <p class="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
            Desenvolvemos soluções inovadoras em web, mobile e desktop que
            impulsionam o sucesso do seu negócio.
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center">
            <Button
              size="lg"
              class="bg-gradient-to-r from-red-600 to-red-700 hover:from-red-700 hover:to-red-800 cursor-pointer transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-xl"
            >
              Começar Projeto
            </Button>
            <Button
              size="lg"
              variant="outline"
              class="border-gray-300 text-gray-700 hover:bg-gray-50 cursor-pointer transform hover:scale-105 transition-all duration-300"
            >
              Ver Portfólio
            </Button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Button } from "@/components/ui/button";
import { Badge } from "@/components/ui/badge";
</script>

<style scoped>
/* Floating animation for background elements */
@keyframes float {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-20px);
  }
}

@keyframes float-slow {
  0%,
  100% {
    transform: translateY(0px) rotate(0deg);
  }
  50% {
    transform: translateY(-15px) rotate(5deg);
  }
}

.animate-float {
  animation: float 6s ease-in-out infinite;
}

.animate-float-slow {
  animation: float-slow 8s ease-in-out infinite;
}
</style>
