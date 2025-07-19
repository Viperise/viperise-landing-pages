<template>
  <section id="contact" class="py-20 px-4 bg-gray-50">
    <div class="container mx-auto text-center">
      <Badge
        variant="secondary"
        class="mb-4 bg-red-100 text-red-700 border-red-200"
      >
        Vamos Conversar
      </Badge>
      <h2
        class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-red-600 to-red-800 bg-clip-text text-transparent"
      >
        Pronto para Começar?
      </h2>
      <p class="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
        Entre em contato conosco e vamos transformar sua ideia em realidade.
        Nossa equipe está pronta para ajudar você a alcançar seus objetivos.
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <Button
          size="lg"
          class="bg-gradient-to-r from-red-600 to-red-700 hover:from-red-700 hover:to-red-800 cursor-pointer transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-xl"
        >
          Solicitar Orçamento
        </Button>
        <Button
          size="lg"
          variant="outline"
          class="border-gray-300 text-gray-700 hover:bg-gray-50 cursor-pointer transform hover:scale-105 transition-all duration-300"
        >
          Agendar Reunião
        </Button>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Button } from "@/components/ui/button";
import { Badge } from "@/components/ui/badge";
</script>
