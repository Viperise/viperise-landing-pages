<template>
  <header
    class="fixed top-0 w-full bg-white/95 backdrop-blur-sm border-b border-gray-200 z-50 shadow-sm"
  >
    <div class="container mx-auto px-4 py-4">
      <div class="flex items-center justify-between">
        <div class="flex items-center space-x-2">
          <img
            src="/viperise-logo-wide.png"
            alt="Viperise"
            class="h-8 w-auto"
          />
        </div>

        <!-- Desktop Navigation -->
        <nav class="hidden md:flex items-center space-x-8">
          <a
            href="#home"
            class="text-gray-600 hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 leading-loose py-1"
            @click="scrollToSection('home')"
            >Início</a
          >
          <a
            href="#services"
            class="text-gray-600 hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 leading-loose py-1"
            @click="scrollToSection('services')"
            >Serviços</a
          >
          <a
            href="#about"
            class="text-gray-600 hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 leading-loose py-1"
            @click="scrollToSection('about')"
            >Sobre</a
          >
          <a
            href="#contact"
            class="text-gray-600 hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 leading-loose py-1"
            @click="scrollToSection('contact')"
            >Contato</a
          >
        </nav>

        <!-- Desktop Button -->
        <Button
          variant="outline"
          class="hidden md:flex border-red-600 text-red-600 hover:bg-red-600 hover:text-white cursor-pointer transform hover:scale-105 transition-all duration-300 leading-loose"
        >
          Fale Conosco
        </Button>

        <!-- Mobile Menu Button -->
        <button
          @click="toggleMobileMenu"
          class="md:hidden p-2 rounded-md text-gray-600 hover:text-red-600 hover:bg-gray-100 transition-all duration-300 transform hover:scale-110 leading-loose"
          aria-label="Abrir menu"
        >
          <div class="relative w-6 h-6">
            <Menu
              v-if="!isMobileMenuOpen"
              class="absolute inset-0 transition-all duration-300 ease-in-out"
              :class="{ 'rotate-90 opacity-0': isMobileMenuOpen }"
            />
            <X
              v-else
              class="absolute inset-0 transition-all duration-300 ease-in-out"
              :class="{ 'rotate-90 opacity-0': !isMobileMenuOpen }"
            />
          </div>
        </button>
      </div>

      <!-- Mobile Menu -->
      <Transition
        enter-active-class="transition-all duration-300 ease-out"
        enter-from-class="opacity-0 transform -translate-y-4"
        enter-to-class="opacity-100 transform translate-y-0"
        leave-active-class="transition-all duration-200 ease-in"
        leave-from-class="opacity-100 transform translate-y-0"
        leave-to-class="opacity-0 transform -translate-y-4"
      >
        <div
          v-show="isMobileMenuOpen"
          class="md:hidden absolute top-full left-0 right-0 bg-white border-b border-gray-200 shadow-lg overflow-hidden"
        >
          <nav class="flex flex-col">
            <TransitionGroup
              enter-active-class="transition-all duration-300 ease-out"
              enter-from-class="opacity-0 transform translate-x-4"
              enter-to-class="opacity-100 transform translate-x-0"
              leave-active-class="transition-all duration-200 ease-in"
              leave-from-class="opacity-100 transform translate-x-0"
              leave-to-class="opacity-0 transform -translate-x-4"
              tag="div"
              class="flex flex-col"
            >
              <a
                key="home"
                href="#home"
                class="px-6 py-4 text-gray-600 hover:text-red-600 hover:bg-gray-50 transition-all duration-200 cursor-pointer border-b border-gray-100 flex items-center leading-loose"
                @click="handleMobileNavClick('home')"
              >
                <span class="flex-1">Início</span>
                <svg
                  class="w-4 h-4 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </a>
              <a
                key="services"
                href="#services"
                class="px-6 py-4 text-gray-600 hover:text-red-600 hover:bg-gray-50 transition-all duration-200 cursor-pointer border-b border-gray-100 flex items-center leading-loose"
                @click="handleMobileNavClick('services')"
              >
                <span class="flex-1">Serviços</span>
                <svg
                  class="w-4 h-4 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </a>
              <a
                key="about"
                href="#about"
                class="px-6 py-4 text-gray-600 hover:text-red-600 hover:bg-gray-50 transition-all duration-200 cursor-pointer border-b border-gray-100 flex items-center leading-loose"
                @click="handleMobileNavClick('about')"
              >
                <span class="flex-1">Sobre</span>
                <svg
                  class="w-4 h-4 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </a>
              <a
                key="contact"
                href="#contact"
                class="px-6 py-4 text-gray-600 hover:text-red-600 hover:bg-gray-50 transition-all duration-200 cursor-pointer border-b border-gray-100 flex items-center leading-loose"
                @click="handleMobileNavClick('contact')"
              >
                <span class="flex-1">Contato</span>
                <svg
                  class="w-4 h-4 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </a>
              <div key="button" class="px-6 py-4">
                <Button
                  variant="outline"
                  class="w-full border-red-600 text-red-600 hover:bg-red-600 hover:text-white transition-all duration-300 transform hover:scale-105 py-3 leading-loose"
                >
                  Fale Conosco
                </Button>
              </div>
            </TransitionGroup>
          </nav>
        </div>
      </Transition>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";
import { Button } from "@/components/ui/button";
import { Menu, X } from "lucide-vue-next";

// Estado reativo para controlar o menu mobile
const isMobileMenuOpen = ref(false);

// Função para alternar o menu mobile
const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};

// Função para lidar com cliques no menu mobile
const handleMobileNavClick = (sectionId) => {
  scrollToSection(sectionId);
  isMobileMenuOpen.value = false; // Fecha o menu após clicar
};

// Smooth scrolling for navigation links
const scrollToSection = (sectionId) => {
  const element = document.getElementById(sectionId);
  if (element) {
    element.scrollIntoView({ behavior: "smooth" });
  }
};
</script>

<style scoped>
/* Animações customizadas */
@keyframes slideDown {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideUp {
  from {
    opacity: 1;
    transform: translateY(0);
  }
  to {
    opacity: 0;
    transform: translateY(-10px);
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}

/* Aplicando animações */
.menu-enter-active {
  animation: slideDown 0.3s ease-out;
}

.menu-leave-active {
  animation: slideUp 0.2s ease-in;
}

.menu-item-enter-active {
  animation: fadeIn 0.3s ease-out;
}

.menu-item-leave-active {
  animation: fadeOut 0.2s ease-in;
}
</style>
