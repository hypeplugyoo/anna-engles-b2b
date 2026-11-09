# ANNA ENGLES — Portal B2B Atacado & Showroom 3D

> Plataforma editorial de atacado (*wholesale*) para boutiques e revendedoras de moda feminina sofisticada. Coleções cápsula em alfaiataria nobre e crepes estruturados, direto de Araras e Leme/SP.

[![Vercel Production](https://img.shields.io/badge/Vercel-Live%20Production-black?style=for-the-badge&logo=vercel)](https://anna-engles-b2b.vercel.app)
[![Three.js](https://img.shields.io/badge/Three.js-WebGL%203D-049EF4?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)
[![License: Proprietary](https://img.shields.io/badge/Licen%C3%A7a-Propriet%C3%A1ria-7A1013?style=for-the-badge)](https://www.annaenglesstore.com.br/)

---

## ✦ Visão Geral

Desenvolvido sob direção de arte editorial de alta-costura (referências: *Vogue*, *Zara Editorial*, *The Row*, *Jacquemus*), este portal B2B foi concebido para transformar a experiência de compras por atacado de lojistas multimarcas:

- **Estética Editorial Sem "Cara de IA"**: Tipografia display personalizada com a fonte **Canesa**, acentos poéticos em **Cormorant Garamond Italic** e precisão arquitetônica em **Montserrat**.
- **Hero 3D em WebGL Reativo**: Simulação física de drapeado de seda pura (*fluid silk satin cloth*) que reage organicamente ao movimento do cursor, scroll e toques mobile em 60 FPS cravados.
- **Catálogo B2B Interativo**:
  - Filtros dinâmicos por categoria (Alfaiataria, Vestidos, Casacos, Blusas, Conjuntos).
  - Variação fluida de cores com *swatches* em tempo real.
  - Cartões com efeito *tilt 3D* e iluminação reativa.
  - Modal editorial de detalhes da peça com grade completa de tamanhos (P, M, G, GG) e cálculo instantâneo de margem de lucro estimada (até 125%).
- **Roteador Comercial de Convites VIP**:
  - Acesso público em modo *Lookbook* com preços sugeridos de revenda e botão de solicitação de credenciamento.
  - Desbloqueio automático de preços de fábrica e faturamento faturado via parâmetros de convite (`?convite=araras-vip`, `?convite=boutique-campinas`).
- **Carrinho & Proforma via WhatsApp**:
  - Barra de progresso dinâmica com rastreamento do Pedido Mínimo de Atacado (**R$ 1.200,00**).
  - Geração de mensagem proforma estruturada para finalização do pedido direto com a diretoria comercial no WhatsApp.
- **Painel Administrativo VIP (`/admin`)**:
  - Protegido por PIN de segurança (`1985`).
  - Gerador de convites personalizados com rastreamento de lojistas por cidade e cópia pré-formatada para prospecção ativa.

---

## ✦ Stack Tecnológica

| Camada | Tecnologia | Propósito |
| :--- | :--- | :--- |
| **Front-end Core** | HTML5 Semântico, CSS Moderno (Design Tokens, Grid Assimétrico) | Estrutura limpa, responsividade em 4 breakpoints e performance máxima |
| **3D & WebGL** | [Three.js r128](https://threejs.org/) | Cena 3D com shaders de tecido, normais dinâmicos e iluminação de estúdio |
| **Motion & Scroll** | [GSAP 3.12](https://greensock.com/gsap/) + [Lenis Scroll](https://lenis.darkroom.engineering/) | Rolagem suave inercial e microinterações editoriais |
| **Tipografia** | **Canesa** (Display OTF) + **Cormorant Garamond** + **Montserrat** | Identidade de luxo, legibilidade refinada e sofisticação visual |
| **Hospedagem & CDN** | [Vercel Edge Network](https://vercel.com) | Clean URLs, compressão Brotli e distribuição global ultrarrápida |

---

## ✦ Estrutura do Repositório

```text
├── index.html          # Aplicação principal (Catálogo B2B, Hero 3D, Carrinho, Lookbook)
├── admin.html          # Painel de Gestão Comercial de Convites VIP (PIN 1985)
├── vercel.json         # Configurações de rotas limpas e cabeçalhos de segurança
├── fonts/
│   └── Canesa-Regular.otf  # Arquivo da fonte tipográfica Canesa
└── README.md           # Documentação completa do projeto
```

---

## ✦ Como Executar Localmente

Como o projeto é construído em tecnologia web nativa sem dependências de compilação pesadas, basta clonar e servir:

```bash
# 1. Clonar o repositório
git clone https://github.com/<SEU_USUARIO>/anna-engles-b2b.git
cd anna-engles-b2b

# 2. Abrir diretamente no navegador ou iniciar um servidor local:
# Com Python 3:
python -m http.server 3000

# Ou com Node.js (npx serve):
npx serve .
```

Acesse em seu navegador:
- **Catálogo / Portal B2B**: `http://localhost:3000/`
- **Acesso VIP Exemplo**: `http://localhost:3000/?convite=araras-vip`
- **Painel Administrativo**: `http://localhost:3000/admin.html` (PIN: `1985`)

---

## ✦ Créditos & Direitos

- **Marca**: [ANNA ENGLES STORE](https://www.annaenglesstore.com.br/) — Araras & Leme, SP.
- **Tipografia Display**: Canesa by Rantau Studio.
