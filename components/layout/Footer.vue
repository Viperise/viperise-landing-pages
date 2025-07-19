<template>
  <footer class="py-12 px-4 border-t border-gray-200 bg-white">
    <div class="container mx-auto">
      <div class="grid md:grid-cols-4 gap-8">
        <div>
          <div class="flex items-center space-x-2 mb-4">
            <img src="/viperise-logo.svg" alt="Viperise" class="h-8 w-auto" />
          </div>
          <p class="text-gray-600">
            Transformando ideias em realidade digital com excelência e inovação.
          </p>
        </div>
        <div>
          <h3 class="text-gray-900 font-semibold mb-4">Serviços</h3>
          <ul class="space-y-2 text-gray-600">
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Desenvolvimento Web</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Desenvolvimento Mobile</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Desenvolvimento Desktop</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Consultoria</a
              >
            </li>
          </ul>
        </div>
        <div>
          <h3 class="text-gray-900 font-semibold mb-4">Empresa</h3>
          <ul class="space-y-2 text-gray-600">
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Sobre Nós</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Portfólio</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Blog</a
              >
            </li>
            <li>
              <a
                href="#"
                class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105 inline-block"
                >Carreiras</a
              >
            </li>
          </ul>
        </div>
        <div>
          <h3 class="text-gray-900 font-semibold mb-4">Contato</h3>
          <ul class="space-y-2 text-gray-600">
            <li>contato@viperise.com</li>
            <li>+55 (11) 99999-9999</li>
            <li>São Paulo, SP</li>
          </ul>
        </div>
      </div>
      <Separator class="my-8 bg-gray-200" />
      <div
        class="flex flex-col md:flex-row justify-between items-center text-gray-600"
      >
        <p>&copy; 2024 Viperise. Todos os direitos reservados.</p>
        <div class="flex space-x-4 mt-4 md:mt-0">
          <a
            href="#"
            class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105"
            >Termos de Uso</a
          >
          <a
            href="#"
            class="hover:text-red-600 transition-colors cursor-pointer transform hover:scale-105"
            >Política de Privacidade</a
          >
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { Separator } from "@/components/ui/separator";
</script>
