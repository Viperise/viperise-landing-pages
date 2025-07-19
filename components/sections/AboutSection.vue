<template>
  <section id="about" class="py-20 px-4 bg-white">
    <div class="container mx-auto">
      <div class="grid md:grid-cols-2 gap-12 items-center">
        <div>
          <Badge
            variant="secondary"
            class="mb-4 bg-red-100 text-red-700 border-red-200"
          >
            Sobre a Viperise
          </Badge>
          <h2
            class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-red-600 to-red-800 bg-clip-text text-transparent"
          >
            Inovação e Excelência
          </h2>
          <p class="text-lg text-gray-600 mb-6">
            Somos uma software house apaixonada por tecnologia e inovação. Nossa
            missão é transformar ideias em soluções digitais que impulsionam o
            sucesso dos nossos clientes.
          </p>
          <div class="space-y-4">
            <div class="flex items-center space-x-3">
              <div
                class="w-8 h-8 bg-red-600 rounded-full flex items-center justify-center"
              >
                <Check class="w-4 h-4 text-white" />
              </div>
              <span class="text-gray-700">Equipe experiente e qualificada</span>
            </div>
            <div class="flex items-center space-x-3">
              <div
                class="w-8 h-8 bg-red-600 rounded-full flex items-center justify-center"
              >
                <Check class="w-4 h-4 text-white" />
              </div>
              <span class="text-gray-700"
                >Tecnologias modernas e atualizadas</span
              >
            </div>
            <div class="flex items-center space-x-3">
              <div
                class="w-8 h-8 bg-red-600 rounded-full flex items-center justify-center"
              >
                <Check class="w-4 h-4 text-white" />
              </div>
              <span class="text-gray-700"
                >Suporte completo e personalizado</span
              >
            </div>
          </div>
        </div>
        <div class="relative">
          <div
            class="bg-gradient-to-r from-red-50 to-red-100 rounded-2xl p-8 border border-red-200"
          >
            <div class="grid grid-cols-2 gap-6">
              <div class="text-center">
                <div class="text-3xl font-bold text-red-600 mb-2">50+</div>
                <div class="text-gray-600">Projetos Entregues</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-red-600 mb-2">30+</div>
                <div class="text-gray-600">Clientes Satisfeitos</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-red-600 mb-2">5+</div>
                <div class="text-gray-600">Anos de Experiência</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-red-600 mb-2">24/7</div>
                <div class="text-gray-600">Suporte Disponível</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Badge } from "@/components/ui/badge";
import { Check } from "lucide-vue-next";
</script>
