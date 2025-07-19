<template>
  <section id="services" class="py-20 px-4 bg-gray-50">
    <div class="container mx-auto">
      <div class="text-center mb-16">
        <Badge
          variant="secondary"
          class="mb-4 bg-red-100 text-red-700 border-red-200"
        >
          Nossos Serviços
        </Badge>
        <h2
          class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-red-600 to-red-800 bg-clip-text text-transparent"
        >
          Soluções Completas
        </h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto">
          Apresentamos aqui uma seleção abrangente dos serviços que
          disponibilizamos para satisfazer as suas necessidades. Nossa gama de
          soluções foi cuidadosamente desenvolvida para atender aos diversos
          desafios e objetivos de nossos clientes, entregando resultados
          excepcionais e impulsionando o sucesso. Explore nossos serviços e
          descubra como podemos colaborar para atingir seus objetivos.
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <!-- Web Development -->
        <Card
          class="bg-white border-gray-200 hover:border-red-300 transition-all duration-300 hover:shadow-lg hover:shadow-red-100"
        >
          <CardHeader>
            <div
              class="w-12 h-12 bg-gradient-to-r from-red-600 to-red-700 rounded-lg flex items-center justify-center mb-4"
            >
              <Globe class="w-6 h-6 text-white" />
            </div>
            <CardTitle class="text-2xl text-gray-900"
              >Desenvolvimento Web</CardTitle
            >
          </CardHeader>
          <CardContent>
            <p class="text-gray-600 mb-4">
              Criamos websites e aplicações web modernas, responsivas e de alta
              performance. Desde landing pages até sistemas complexos de
              e-commerce e dashboards empresariais.
            </p>
            <div class="space-y-2">
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Sites Responsivos</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">E-commerce</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Dashboards</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">APIs RESTful</span>
              </div>
            </div>
          </CardContent>
          <CardFooter>
            <Button
              variant="outline"
              class="w-full border-red-600 text-red-600 hover:bg-red-600 hover:text-white cursor-pointer transform hover:scale-105 transition-all duration-300"
            >
              Saiba Mais
            </Button>
          </CardFooter>
        </Card>

        <!-- Mobile Development -->
        <Card
          class="bg-white border-gray-200 hover:border-red-300 transition-all duration-300 hover:shadow-lg hover:shadow-red-100"
        >
          <CardHeader>
            <div
              class="w-12 h-12 bg-gradient-to-r from-red-600 to-red-700 rounded-lg flex items-center justify-center mb-4"
            >
              <Smartphone class="w-6 h-6 text-white" />
            </div>
            <CardTitle class="text-2xl text-gray-900"
              >Desenvolvimento Mobile</CardTitle
            >
          </CardHeader>
          <CardContent>
            <p class="text-gray-600 mb-4">
              Desenvolvemos aplicativos nativos e híbridos para iOS e Android.
              Focamos em experiência do usuário excepcional e performance
              otimizada.
            </p>
            <div class="space-y-2">
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">iOS Nativo</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Android Nativo</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">React Native</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Flutter</span>
              </div>
            </div>
          </CardContent>
          <CardFooter>
            <Button
              variant="outline"
              class="w-full border-red-600 text-red-600 hover:bg-red-600 hover:text-white cursor-pointer transform hover:scale-105 transition-all duration-300"
            >
              Saiba Mais
            </Button>
          </CardFooter>
        </Card>

        <!-- Desktop Development -->
        <Card
          class="bg-white border-gray-200 hover:border-red-300 transition-all duration-300 hover:shadow-lg hover:shadow-red-100"
        >
          <CardHeader>
            <div
              class="w-12 h-12 bg-gradient-to-r from-red-600 to-red-700 rounded-lg flex items-center justify-center mb-4"
            >
              <Monitor class="w-6 h-6 text-white" />
            </div>
            <CardTitle class="text-2xl text-gray-900"
              >Desenvolvimento Desktop</CardTitle
            >
          </CardHeader>
          <CardContent>
            <p class="text-gray-600 mb-4">
              Criamos aplicações desktop robustas e eficientes para Windows,
              macOS e Linux. Soluções empresariais que otimizam processos e
              aumentam produtividade.
            </p>
            <div class="space-y-2">
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Windows</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">macOS</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Linux</span>
              </div>
              <div class="flex items-center space-x-2">
                <div class="w-2 h-2 bg-red-500 rounded-full"></div>
                <span class="text-sm text-gray-500">Electron</span>
              </div>
            </div>
          </CardContent>
          <CardFooter>
            <Button
              variant="outline"
              class="w-full border-red-600 text-red-600 hover:bg-red-600 hover:text-white cursor-pointer transform hover:scale-105 transition-all duration-300"
            >
              Saiba Mais
            </Button>
          </CardFooter>
        </Card>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Button } from "@/components/ui/button";
import {
  Card,
  CardContent,
  CardFooter,
  CardHeader,
  CardTitle,
} from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";
import { Globe, Smartphone, Monitor } from "lucide-vue-next";
</script>
