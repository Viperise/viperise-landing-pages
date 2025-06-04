<template>
  <header
    class="fixed top-0 left-0 right-0 z-50 border-b bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60"
  >
    <div
      class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex h-16 items-center justify-between"
    >
      <div class="flex items-center gap-2">
        <img src="/reachout-logo.svg" alt="Reachout Logo" class="h-8" />
      </div>

      <!-- Desktop Navigation -->
      <nav class="hidden md:flex items-center gap-6">
        <a
          href="#"
          class="text-sm font-medium transition-colors hover:text-primary"
          >Início</a
        >
        <a
          href="#"
          class="text-sm font-medium transition-colors hover:text-primary"
          >Recursos</a
        >
        <a
          href="#"
          class="text-sm font-medium transition-colors hover:text-primary"
          >Preços</a
        >
        <a
          href="#"
          class="text-sm font-medium transition-colors hover:text-primary"
          >Sobre</a
        >
      </nav>

      <div class="hidden md:flex items-center gap-4">
        <Button variant="ghost">Entrar</Button>
        <Button>Começar Agora</Button>
      </div>

      <!-- Mobile Menu Button -->
      <Button variant="ghost" size="icon" class="md:hidden" @click="isMenuOpen = !isMenuOpen">
        <Menu v-if="!isMenuOpen" class="h-5 w-5" />
        <X v-else class="h-5 w-5" />
      </Button>
    </div>

    <!-- Mobile Navigation -->
    <Transition
      enter-active-class="transition duration-200 ease-out"
      enter-from-class="transform scale-95 opacity-0"
      enter-to-class="transform scale-100 opacity-100"
      leave-active-class="transition duration-150 ease-in"
      leave-from-class="transform scale-100 opacity-100"
      leave-to-class="transform scale-95 opacity-0"
    >
      <div
        v-if="isMenuOpen"
        class="absolute top-16 left-0 right-0 bg-background border-b p-4 md:hidden"
      >
        <nav class="flex flex-col gap-4">
          <a
            href="#"
            class="text-sm font-medium transition-colors hover:text-primary"
            >Início</a
          >
          <a
            href="#"
            class="text-sm font-medium transition-colors hover:text-primary"
            >Recursos</a
          >
          <a
            href="#"
            class="text-sm font-medium transition-colors hover:text-primary"
            >Preços</a
          >
          <a
            href="#"
            class="text-sm font-medium transition-colors hover:text-primary"
            >Sobre</a
          >
          <div class="flex flex-col gap-2 pt-2 border-t">
            <Button variant="ghost" class="w-full justify-start">Entrar</Button>
            <Button class="w-full justify-start">Começar Agora</Button>
          </div>
        </nav>
      </div>
    </Transition>
  </header>
</template>

<script setup>
import { ref } from "vue";
import { Button } from "@/components/ui/button";
import { Menu, X } from "lucide-vue-next";

const isMenuOpen = ref(false);
</script>
