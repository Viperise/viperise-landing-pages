<template>
  <section class="py-20 bg-background">
    <div class="container mx-auto px-4">
      <h2 class="text-4xl font-bold text-center mb-4">Planos e Preços</h2>
      <p class="text-center text-gray-600 mb-12 max-w-2xl mx-auto">
        Escolha o plano ideal para o seu negócio e comece a expandir sua
        presença digital hoje mesmo.
      </p>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <!-- Plano Básico -->
        <div class="bg-white rounded-lg shadow-lg p-8 border border-gray-200">
          <h3 class="text-2xl font-bold mb-4">Básico</h3>
          <div class="mb-6">
            <span class="text-4xl font-bold">R$ 79,90</span>
            <span class="text-gray-600">/mês</span>
          </div>
          <ul class="space-y-4 mb-8">
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              1 usuário
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Até 5 anúncios/mês
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Suporte básico
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Painel simples
            </li>
          </ul>
          <button
            class="w-full bg-primary text-white py-3 rounded-lg hover:bg-primary/90 transition-colors cursor-pointer"
          >
            Começar agora
          </button>
        </div>

        <!-- Plano Profissional -->
        <div
          class="bg-white rounded-lg shadow-lg p-8 border-2 border-primary relative"
        >
          <div
            class="absolute -top-4 left-1/2 transform -translate-x-1/2 bg-primary text-white px-4 py-1 rounded-full text-sm text-center"
          >
            Mais popular
          </div>
          <h3 class="text-2xl font-bold mb-4">Profissional</h3>
          <div class="mb-6">
            <span class="text-4xl font-bold text-primary">R$ 149,98</span>
            <span class="text-gray-600">/mês</span>
          </div>
          <ul class="space-y-4 mb-8">
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              3 usuários
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Até 50 anúncios/mês
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Agendamento de anúncios
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Tudo do plano Básico
            </li>
          </ul>
          <button
            class="w-full bg-primary text-white py-3 rounded-lg hover:bg-primary/90 transition-colors cursor-pointer"
          >
            Começar agora
          </button>
        </div>

        <!-- Plano Agência -->
        <div class="bg-white rounded-lg shadow-lg p-8 border border-gray-200">
          <h3 class="text-2xl font-bold mb-4">Agência</h3>
          <div class="mb-6">
            <span class="text-4xl font-bold">R$ 299,99</span>
            <span class="text-gray-600">/mês</span>
          </div>
          <ul class="space-y-4 mb-8">
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Usuários ilimitados
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Até 200 anúncios/mês
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Branding próprio
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Tudo do plano Profissional
            </li>
          </ul>
          <button
            class="w-full bg-primary text-white py-3 rounded-lg hover:bg-primary/90 transition-colors cursor-pointer"
          >
            Começar agora
          </button>
        </div>

        <!-- Plano Enterprise -->
        <div class="bg-white rounded-lg shadow-lg p-8 border border-gray-200">
          <h3 class="text-2xl font-bold mb-4">Enterprise</h3>
          <div class="mb-6">
            <span class="text-4xl font-bold">A consultar</span>
          </div>
          <ul class="space-y-4 mb-8">
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Integrações exclusivas
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Limite personalizado
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              SLA de suporte
            </li>
            <li class="flex items-center">
              <svg
                class="w-5 h-5 text-green-500 mr-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M5 13l4 4L19 7"
                ></path>
              </svg>
              Soluções personalizadas
            </li>
          </ul>
          <button
            class="w-full bg-primary text-white py-3 rounded-lg hover:bg-primary/90 transition-colors cursor-pointer"
          >
            Fale conosco
          </button>
        </div>
      </div>

      <!-- Observação sobre pacotes de dispositivos -->
      <div class="mt-16 bg-gray-50 rounded-lg p-8 text-center">
        <h3 class="text-2xl font-bold mb-4">Pacotes de Dispositivos</h3>
        <p class="text-gray-600 mb-6">
          Oferecemos pacotes especiais de tablets com o sistema de cardápio e
          anúncios pré-instalados. Para mais informações sobre preços e
          disponibilidade, entre em contato conosco pelo WhatsApp.
        </p>
        <a
          href="https://wa.me/seu-numero"
          class="inline-flex items-center bg-green-500 text-white px-6 py-3 rounded-lg hover:bg-green-600 transition-colors cursor-pointer"
        >
          <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"
            />
          </svg>
          Fale conosco no WhatsApp
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
// Componente de preços
</script>
