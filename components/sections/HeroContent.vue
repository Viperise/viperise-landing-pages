<template>
  <div class="flex flex-col justify-center space-y-6 md:space-y-8">
    <div class="space-y-4">
      <h1
        class="text-4xl font-bold tracking-tighter sm:text-5xl md:text-6xl lg:text-7xl"
      >
        Cardápio Digital Inteligente
      </h1>
      <p
        class="text-base sm:text-lg md:text-xl text-muted-foreground max-w-[600px]"
      >
        Transforme a experiência dos seus clientes com um cardápio digital
        interativo. Faça pedidos online, descubra promoções personalizadas e
        aumente suas vendas com anúncios de alta conversão.
      </p>
    </div>
    <div class="flex flex-col sm:flex-row gap-4">
      <Button size="lg" class="w-full sm:w-auto"> Experimente Agora </Button>
      <Button size="lg" variant="outline" class="w-full sm:w-auto">
        Ver Demonstração
      </Button>
    </div>
  </div>
</template>

<script setup>
import { Button } from "@/components/ui/button";
</script>
