# Componentes da Viperise Landing Pages

Esta pasta contém todos os componentes reutilizáveis do projeto, organizados por categoria.

## Estrutura

```
components/
├── layout/           # Componentes de layout (Header, Footer)
├── sections/         # Seções da página (Hero, Services, About, etc.)
├── ui/              # Componentes de interface (Button, Card, Badge, etc.)
└── README.md        # Este arquivo
```

## Layout Components

### Header

- **Arquivo**: `layout/Header.vue`
- **Descrição**: Cabeçalho fixo com navegação e logo
- **Funcionalidades**: Navegação suave, logo da Viperise, botão de contato

### Footer

- **Arquivo**: `layout/Footer.vue`
- **Descrição**: Rodapé com informações da empresa e links
- **Funcionalidades**: Links de serviços, empresa, contato, termos de uso

## Section Components

### HeroSection

- **Arquivo**: `sections/HeroSection.vue`
- **Descrição**: Seção principal com título e call-to-action
- **Funcionalidades**: Animações de fundo, gradientes, botões de ação

### ServicesSection

- **Arquivo**: `sections/ServicesSection.vue`
- **Descrição**: Seção de serviços oferecidos
- **Funcionalidades**: Cards de serviços (Web, Mobile, Desktop)

### AboutSection

- **Arquivo**: `sections/AboutSection.vue`
- **Descrição**: Seção sobre a empresa
- **Funcionalidades**: Estatísticas, lista de benefícios

### ContactSection

- **Arquivo**: `sections/ContactSection.vue`
- **Descrição**: Seção de contato e call-to-action
- **Funcionalidades**: Botões de orçamento e agendamento

## Como Usar

### Importação Individual

```vue
<script setup>
import Header from "@/components/layout/Header.vue";
import HeroSection from "@/components/sections/HeroSection.vue";
</script>
```

### Importação em Lote

```vue
<script setup>
import { Header, Footer } from "@/components/layout";
import { HeroSection, ServicesSection } from "@/components/sections";
</script>
```

## Customização

Cada componente pode ser customizado através de:

- Props (quando implementadas)
- Classes CSS
- Slots (quando implementados)
- Eventos (quando implementados)

## Estilo

Todos os componentes seguem o design system da Viperise:

- Cores: Vermelho (#dc2626) como cor principal
- Tipografia: Poppins
- Animações: Transições suaves e hover effects
- Responsividade: Mobile-first approach
