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
      <Button variant="ghost" size="icon" class="md:hidden">
        <Menu class="h-5 w-5" />
      </Button>
    </div>
  </header>
</template>

<script setup>
import { Button } from "@/components/ui/button";
import { Menu } from "lucide-vue-next";
</script>
