# LAR ARQUITETURA - Landing Page

Crie uma landing page premium e minimalista para a Lar Arquitetura, um escritório de arquitetura estratégica para incorporação com mais de 30 anos de atuação em Maringá/PR. O design deve ser sofisticado, clean e com muito espaço em branco. Idioma: PT-BR.

## DESIGN SYSTEM (design.json)

```json
{
  "designSystem": {
    "name": "Lar Arquitetura Design System",
    "version": "1.0",
    "description": "Design minimalista e premium para escritório de arquitetura — sofisticação, espaço em branco generoso e tipografia elegante"
  },

  "designPrinciples": [
    {
      "name": "Espaço como elemento",
      "description": "O espaço em branco é tão importante quanto o conteúdo. Cada seção deve respirar."
    },
    {
      "name": "Sofisticação silenciosa",
      "description": "Transmitir autoridade sem exagero. Tipografia elegante, cores neutras, transições suaves."
    },
    {
      "name": "Arquitetura no design",
      "description": "O layout do site deve refletir os mesmos princípios da boa arquitetura: proporção, ritmo e propósito."
    }
  ],

  "colors": {
    "primary": {
      "main": "#1A1A1A",
      "light": "#333333",
      "dark": "#0D0D0D",
      "description": "Cor principal para textos, headers e elementos âncora. Transmite seriedade e sofisticação."
    },
    "accent": {
      "main": "#C9A96E",
      "hover": "#B8944F",
      "light": "#E8D5B0",
      "description": "Dourado sutil para CTAs, destaques e elementos de ênfase. Transmite premium sem ostentação."
    },
    "background": {
      "white": "#FFFFFF",
      "cream": "#FAFAF7",
      "warmGray": "#F5F3EF",
      "dark": "#1A1A1A",
      "description": "Alternar entre white e cream/warmGray entre seções para criar ritmo visual."
    },
    "text": {
      "primary": "#1A1A1A",
      "secondary": "#5C5C5C",
      "muted": "#8A8A8A",
      "onDark": "#FAFAF7",
      "description": "Hierarquia clara: primary para títulos, secondary para corpo, muted para labels."
    },
    "ui": {
      "border": "#E5E2DC",
      "shadow": "rgba(0,0,0,0.06)",
      "divider": "#E5E2DC",
      "success": "#4A7C59"
    }
  },

  "typography": {
    "fontFamily": {
      "heading": "'Playfair Display', Georgia, serif",
      "body": "'Inter', system-ui, sans-serif"
    },
    "headings": {
      "h1": {
        "size": "clamp(2.5rem, 5vw, 4rem)",
        "weight": "400",
        "lineHeight": "1.1",
        "letterSpacing": "-0.02em",
        "note": "Peso leve para elegância. Usar italic para ênfase em palavras-chave."
      },
      "h2": {
        "size": "clamp(2rem, 4vw, 3rem)",
        "weight": "400",
        "lineHeight": "1.2",
        "letterSpacing": "-0.01em"
      },
      "h3": {
        "size": "1.25rem",
        "weight": "600",
        "lineHeight": "1.4",
        "fontFamily": "'Inter', system-ui, sans-serif"
      }
    },
    "body": {
      "large": { "size": "1.125rem", "lineHeight": "1.8" },
      "base": { "size": "1rem", "lineHeight": "1.7" },
      "small": { "size": "0.875rem", "lineHeight": "1.5" }
    },
    "special": {
      "eyebrow": {
        "size": "0.75rem",
        "weight": "600",
        "letterSpacing": "0.15em",
        "textTransform": "uppercase",
        "fontFamily": "'Inter', sans-serif",
        "color": "#C9A96E"
      }
    }
  },

  "spacing": {
    "section": {
      "paddingY": "clamp(5rem, 12vw, 10rem)",
      "paddingX": "clamp(1.5rem, 5vw, 4rem)"
    },
    "container": { "maxWidth": "1100px" },
    "grid": { "gap": "3rem", "cardGap": "2rem" }
  },

  "components": {
    "buttons": {
      "primary": {
        "background": "#C9A96E",
        "text": "#FFFFFF",
        "borderRadius": "0px",
        "paddingX": "2.5rem",
        "paddingY": "1rem",
        "fontWeight": "500",
        "fontSize": "0.875rem",
        "letterSpacing": "0.1em",
        "textTransform": "uppercase",
        "hoverBackground": "#B8944F",
        "hoverTransform": "none",
        "transition": "all 0.3s ease",
        "note": "Botões retangulares (sem border-radius) para reforçar estética arquitetônica."
      },
      "secondary": {
        "background": "transparent",
        "text": "#1A1A1A",
        "border": "1px solid #1A1A1A",
        "borderRadius": "0px",
        "hoverBackground": "#1A1A1A",
        "hoverText": "#FFFFFF"
      }
    },
    "cards": {
      "default": {
        "background": "#FFFFFF",
        "borderRadius": "0px",
        "padding": "2.5rem",
        "boxShadow": "none",
        "border": "1px solid #E5E2DC",
        "hoverBorder": "1px solid #C9A96E",
        "transition": "all 0.3s ease"
      }
    },
    "dividers": {
      "thin": "1px solid #E5E2DC",
      "accent": "2px solid #C9A96E",
      "note": "Usar linhas finas como elemento arquitetônico de separação."
    }
  },

  "effects": {
    "shadows": {
      "sm": "0 1px 3px rgba(0,0,0,0.04)",
      "md": "0 4px 12px rgba(0,0,0,0.06)",
      "lg": "0 10px 40px rgba(0,0,0,0.08)"
    },
    "transitions": {
      "default": "all 0.3s ease",
      "smooth": "all 0.5s cubic-bezier(0.4, 0, 0.2, 1)"
    }
  },

  "responsive": {
    "breakpoints": {
      "sm": "640px",
      "md": "768px",
      "lg": "1024px",
      "xl": "1280px"
    },
    "mobileAdaptations": [
      "Single column layouts",
      "Reduced heading sizes",
      "Full-width buttons",
      "Hamburger navigation com overlay escuro"
    ]
  }
}
```

---

## ESPECIFICAÇÕES POR SEÇÃO

### Seção 1: Hero

**Layout:** 2 colunas (50% texto / 50% imagem) — imagem full-height à direita
**Background:** #FFFFFF

#### Coluna Esquerda
- **Eyebrow:** "ARQUITETURA ESTRATÉGICA" — uppercase, Inter 600, 0.75rem, cor #C9A96E, letter-spacing 0.15em
- **Título h1:** "Seu empreendimento merece uma arquitetura que *vende*"
  - Playfair Display 400, clamp(2.5rem, 5vw, 4rem)
  - A palavra "vende" em itálico (Playfair Display Italic) + cor gold (#C9A96E) para ênfase elegante
- **Subtítulo:** "Há 30 anos, criamos projetos que diferenciam incorporadoras no mercado — com estudo de viabilidade antes do primeiro traço e design autoral que gera identidade."
  - Inter 400, #5C5C5C, 1.125rem, max-width 500px, line-height 1.8
- **CTA:** "AGENDE UMA CONVERSA"
  - Botão retangular, #C9A96E bg, branco texto, uppercase, letter-spacing 0.1em
- **Indicador:** "30+ anos de atuação · Maringá e outros estados" — Inter 400, #8A8A8A, 0.875rem

#### Coluna Direita
- Imagem full-height de arquitetura moderna
- Usar imagem do Unsplash de fachada arquitetônica contemporânea e clean (buscar "modern architecture building facade minimal")
- Aplicar leve overlay escuro (rgba(0,0,0,0.05)) para suavizar
- object-fit: cover

#### Animações
- Texto: fade-in-up sequencial (title → subtitle → CTA), 0.6s ease, 0.15s delay entre cada
- Imagem: fade-in com leve scale (1.05 → 1.0), 0.8s ease

---

### Seção 2: Prova Social / Números

**Layout:** 4 colunas com números centralizados
**Background:** #FAFAF7
**Divider:** linha fina (#E5E2DC) top e bottom

#### Conteúdo
| Número | Label |
|--------|-------|
| 30+ | Anos de atuação |
| 200+ | Projetos entregues |
| 15+ | Cidades atendidas |
| 50+ | Incorporadoras parceiras |

*Nota: substituir por números reais do cliente*

- Números: Playfair Display 400, 3rem, #1A1A1A
- Labels: Inter 400, 0.875rem, #8A8A8A, uppercase, letter-spacing 0.1em
- Separador vertical fino entre cada coluna (desktop)

#### Animações
- Números: count-up animation ao entrar na viewport
- Colunas: stagger fade-in (0.1s delay)

---

### Seção 3: Por que a Lar

**Layout:** Título centralizado + grid 2x2 de cards abaixo
**Background:** #FFFFFF

#### Header
- **Eyebrow:** "POR QUE NOS ESCOLHER"
- **Título h2:** "Mais do que um escritório de arquitetura"

#### Cards (grid 2x2)

**Card 1: Investimento seguro desde o dia zero**
- Ícone: linha fina de gráfico/análise (Lucide: BarChart3)
- Descrição: "Analisamos viabilidade técnica e financeira antes do primeiro traço. Seu investimento começa seguro."

**Card 2: Projetos que fazem sentido no contexto**
- Ícone: linha fina de mapa/bússola (Lucide: Compass)
- Descrição: "Lemos o contexto urbano, cultural e econômico para projetar com precisão e relevância."

**Card 3: Empreendimentos que se vendem pela fachada**
- Ícone: linha fina de cubo/forma geométrica (Lucide: Box)
- Descrição: "Projetos com identidade própria que geram valor simbólico e diferenciação no mercado."

**Card 4: Um parceiro do estudo à entrega**
- Ícone: linha fina de setas conectadas (Lucide: ArrowRightLeft)
- Descrição: "Do estudo de viabilidade ao projeto final. Um parceiro em todas as etapas."

- Cards: fundo branco, borda 1px #E5E2DC, padding 2.5rem, sem border-radius
- Hover: borda muda para #C9A96E, transição 0.3s

#### Animações
- Cards: stagger fade-in-up on scroll

---

### Seção 4: Serviços

**Layout:** Seções alternadas (imagem esquerda/direita + texto)
**Background:** #FAFAF7

#### Header
- **Eyebrow:** "NOSSOS SERVIÇOS"
- **Título h2:** "Do estudo à entrega, com propósito em cada etapa"

#### Serviço 1: Estudo de Viabilidade
- **Layout:** Imagem à esquerda (50%), texto à direita (50%)
- **Imagem Unsplash:** buscar "architectural blueprints analysis" ou "real estate development planning"
- **Título h3:** "Decisões seguras antes do primeiro investimento"
- **Descrição:** "Avaliamos orçamento, localização, regulamentações e requisitos técnicos para garantir que seu projeto é viável e rentável."
- **Detalhe:** linha accent (#C9A96E, 40px de largura) acima do título

#### Serviço 2: Urbanismo
- **Layout:** Texto à esquerda (50%), imagem à direita (50%)
- **Imagem Unsplash:** buscar "urban planning aerial view modern city" ou "masterplan architecture"
- **Título h3:** "Grandes áreas, soluções inteligentes"
- **Descrição:** "Desenvolvemos projetos urbanísticos sustentáveis, funcionais e alinhados com as dinâmicas locais e comunitárias."

#### Serviço 3: Arquitetura
- **Layout:** Imagem à esquerda (50%), texto à direita (50%)
- **Imagem Unsplash:** buscar "modern residential building architecture" ou "contemporary architecture exterior"
- **Título h3:** "Projetos autorais que criam identidade"
- **Descrição:** "Combinamos visão criativa, técnicas avançadas de modelagem e leitura de território para criar projetos exclusivos que geram valor simbólico e de mercado."

#### Animações
- Cada serviço: fade-in-up on scroll
- Imagens: leve parallax (velocidade 0.95)

---

### Seção 4.5: Portfólio de Projetos

**Layout:** Grid filtrado por categorias com painel de detalhes expansível
**Background:** #FFFFFF
**Posição:** Entre Serviços e Como Trabalhamos

#### Header
- **Eyebrow:** "PORTFÓLIO"
- **Título h2:** "Projetos que geram *identidade*"
  - Playfair Display 400, italic + gold (#C9A96E) na palavra "identidade"

#### Filtro de Categorias
- Barra horizontal com 5 tabs: **TODOS** | **CASAS** | **COMÉRCIOS** | **INTERIORES** | **EDIFÍCIOS**
- Tab ativa: texto #1A1A1A + underline animado gold (#C9A96E, 2px) que desliza via Framer Motion `layoutId`
- Tab inativa: texto #7A7A7A, hover → #1A1A1A
- Estilo: Inter 600, 0.75rem, uppercase, letter-spacing 0.15em
- Mobile: scroll horizontal com scrollbar escondida

#### Grid de Thumbnails (3 colunas)
- CSS Grid: `grid-cols-1 md:grid-cols-2 lg:grid-cols-3`, gap 1rem
- Cada thumbnail:
  - Container overflow-hidden, aspect-ratio 4:3
  - Hover: imagem scale 1.0 → 1.08 (transition 0.5s)
  - Overlay escuro (rgba(0,0,0,0.3)) aparece no hover
  - Nome do projeto revelado no hover (branco, Playfair, bottom-left)
  - Tag de categoria no hover (eyebrow gold, top-left)
  - Projeto selecionado: ring gold (2px #C9A96E)
- AnimatePresence para transição suave ao filtrar categorias
- Stagger entrance animation

#### Painel de Detalhes (expansível)
- Abre abaixo do grid ao clicar em um projeto
- Animação: height 0 → auto + opacity (spring physics)
- Layout 2 colunas (desktop):
  - **Esquerda (38%):** nome do projeto (Playfair h3), tag de categoria (eyebrow), descrição (Inter body), linha gold accent
  - **Direita (62%):** galeria horizontal scroll (snap-x snap-mandatory)
- Galeria:
  - Imagens em aspect-ratio 16:9 com overflow-hidden
  - Navegação: setas esquerda/direita + counter "01 / 12"
  - Scrollbar escondida
- Botão fechar (X) no topo-direito
- Scroll automático até o painel ao abrir
- Mobile: empilha verticalmente — info topo, galeria full-width abaixo
- Background: #FAFAF7, borda-top #E5E2DC

#### Projetos (20 total)

| Categoria | Projetos |
|-----------|----------|
| **Casas** | Casa LF, Casa PN |
| **Interiores** | Apartamento MN, Dell Anno |
| **Comércios** | Box One Fitness, Carnívoros, Casablanca Hall, Colli Bike, Country Club Complexo Piscinas, Fabrílo Rosa e Trovão Advogados, Grupo GTFoods, Jardins de Monet Centro de Esportes, Jardins de Monet Salão de Festas |
| **Edifícios** | 54 Park Square, Condomínio Villagio Bourbon, Edifício El Cielo, Edifício Le Monde, Edifício Unikue Marechal, Edifício Vital, TAJ Condomínio Resort |

*Imagens reais da empresa em `public/images/portfolio/` (uma subpasta por projeto)*

#### Animações
- Filtro: underline gold desliza com shared layout animation
- Grid: AnimatePresence com fade + scale (0.96 → 1.0) ao filtrar
- Painel: spring height animation (stiffness 300, damping 35)
- Galeria: scroll horizontal com snap

---

### Seção 5: Como Trabalhamos

**Layout:** 4 passos em linha horizontal (desktop) / vertical (mobile)
**Background:** #FFFFFF

#### Header
- **Eyebrow:** "NOSSO PROCESSO"
- **Título h2:** "Arquitetura com método e propósito"

#### Passos

**Passo 1 — Escuta e Leitura**
- Número: "01" em Playfair Display, #C9A96E
- Descrição: "Entendemos seu objetivo, lemos o território e mapeamos o contexto urbano, cultural e econômico."

**Passo 2 — Viabilidade e Estratégia**
- Número: "02"
- Descrição: "Analisamos viabilidade técnica e financeira para garantir decisões seguras."

**Passo 3 — Projeto Autoral**
- Número: "03"
- Descrição: "Desenvolvemos o projeto com design autoral, técnica e foco na experiência."

**Passo 4 — Acompanhamento e Entrega**
- Número: "04"
- Descrição: "Gerimos cada etapa com excelência, tecnologia e evolução constante."

- Linha conectora fina (#E5E2DC) entre os passos (horizontal desktop, vertical mobile)

#### Animações
- Passos: stagger reveal on scroll (0.15s delay)
- Linha: draw animation da esquerda para direita
- Números: fade-in com leve scale

---

### Seção 6: Depoimentos

**Layout:** 3 colunas de cards
**Background:** #FAFAF7

#### Header
- **Eyebrow:** "DEPOIMENTOS"
- **Título h2:** "Quem confia na Lar"

#### Cards

**Card 1:**
- Aspas: ícone " em #C9A96E, 20% opacity, canto superior esquerdo
- Quote: "A Lar não entrega apenas um projeto — entrega uma estratégia. O estudo de viabilidade nos deu segurança para investir, e o resultado superou expectativas."
- Nome: "Roberto Mendes"
- Role: "Diretor de Incorporação"
- [SUGESTÃO - substituir por depoimento real se disponível]

**Card 2:**
- Quote: "Trabalhávamos com escritórios que entregavam plantas eficientes, mas sem identidade. Com a Lar, nossos empreendimentos passaram a se destacar no mercado."
- Nome: "Fernanda Almeida"
- Role: "CEO de Incorporadora"
- [SUGESTÃO - substituir por depoimento real]

**Card 3:**
- Quote: "O diferencial da Lar é a leitura que fazem do território. Eles entendem o contexto e projetam para ele. Isso é raro."
- Nome: "Marcos Oliveira"
- Role: "Investidor Imobiliário"
- [SUGESTÃO - substituir por depoimento real]

- Card style: branco, borda fina #E5E2DC, padding 2.5rem, sem border-radius
- Quote text: Inter 400, 1rem, #5C5C5C, italic
- Nome: Inter 600, #1A1A1A
- Role: Inter 400, #8A8A8A

#### Animações
- Cards: stagger fade-in (0.15s delay)

---

### Seção 7: Para Quem

**Layout:** 3 colunas
**Background:** #FFFFFF

#### Header
- **Eyebrow:** "PARA QUEM PROJETAMOS"
- **Título h2:** "Parceiros que buscam mais do que edificações"

#### Cards

**Card 1: Incorporadoras**
- Ícone: Building/prédio em linha fina (Lucide: Building2)
- Descrição: "Que querem empreendimentos com identidade própria e diferenciação no mercado."

**Card 2: Investidores Imobiliários**
- Ícone: TrendingUp/gráfico em linha fina (Lucide: TrendingUp)
- Descrição: "Que precisam de segurança no investimento e projetos que geram valor real."

**Card 3: Desenvolvedores Urbanos**
- Ícone: Map/Globe em linha fina (Lucide: Globe)
- Descrição: "Que buscam soluções urbanísticas sustentáveis e integradas ao contexto local."

#### Animações
- Cards: stagger fade-in-up

---

### Seção 8: CTA Final

**Layout:** Centralizado, max-width 700px
**Background:** #1A1A1A (dark)
**Texto:** #FAFAF7

#### Conteúdo
- **Título h2:** "Seu próximo empreendimento merece *mais* que plantas eficientes"
  - Playfair Display 400, branco, italic na palavra "mais"
- **Lista de benefícios:**
  - ✓ Mais de 30 anos de experiência e visão contemporânea
  - ✓ Estudo de viabilidade integrado ao processo
  - ✓ Arquitetura autoral que gera valor de mercado
  - Checkmarks em #C9A96E
- **CTA:** "AGENDE UMA CONVERSA" — botão com borda #C9A96E, texto branco, hover: bg #C9A96E

#### Animações
- Seção: fade-in on scroll
- Checkmarks: stagger pop-in (0.1s delay)

---

### Seção 9: FAQ

**Layout:** Accordion centralizado, max-width 800px
**Background:** #FAFAF7

#### Header
- **Título h2:** "Perguntas frequentes"

#### Perguntas

**Q1:** "Qual a diferença entre a Lar e outros escritórios de arquitetura?"
**A1:** "Não entregamos apenas projetos — entregamos estratégia. Combinamos estudo de viabilidade, leitura de território e arquitetura autoral para criar empreendimentos que geram identidade e valor de mercado."

**Q2:** "Vocês atendem fora de Maringá?"
**A2:** "Sim. Atuamos em Maringá, região e outros estados, sempre com a mesma excelência e proximidade."

**Q3:** "O que é o estudo de viabilidade?"
**A3:** "É uma análise completa de orçamento, localização, regulamentações e requisitos técnicos que fazemos antes do início do projeto, para garantir que seu investimento é viável e rentável."

**Q4:** "Quanto tempo leva um projeto?"
**A4:** "Depende da complexidade e escopo. Em nossa reunião inicial, apresentamos um cronograma detalhado e transparente para cada etapa."

**Q5:** "Vocês trabalham com projetos residenciais?"
**A5:** "Nosso foco principal é em incorporadoras e investidores, mas avaliamos cada oportunidade. Entre em contato para conversarmos sobre seu projeto."

**Q6:** "O investimento em arquitetura autoral é mais alto?"
**A6:** "Nosso processo integrado elimina retrabalhos e surpresas. Incorporadoras que investem em identidade arquitetônica reportam maior velocidade de vendas e valorização do m². O retorno justifica o investimento."

- Accordion: borda-bottom #E5E2DC, chevron à direita
- Transição suave (height 0.3s ease)

---

### Seção 10: Footer

**Layout:** 4 colunas
**Background:** #1A1A1A
**Texto:** #FAFAF7

#### Colunas

**Coluna 1: Marca**
- Logo Lar Arquitetura (branco/invertido)
- "Arquitetura estratégica para incorporação" — #8A8A8A, 0.875rem

**Coluna 2: Navegação**
- Sobre
- Serviços
- Portfólio
- Contato

**Coluna 3: Serviços**
- Estudo de Viabilidade
- Urbanismo
- Arquitetura

**Coluna 4: Contato**
- Endereço em Maringá
- Telefone
- Email
- Instagram | LinkedIn

#### Bottom Bar
- Divider: 1px solid #333333
- "© 2026 Lar Arquitetura. Todos os direitos reservados."
- CREA badge (se aplicável)

---

## NOTAS IMPORTANTES DE ESTILO

1. **Whitespace:** Espaçamento muito generoso entre seções (clamp 5rem-10rem). O vazio é elegância.
2. **Tipografia:** Playfair Display para títulos (peso 400, usar italic para ênfase). Inter para corpo.
3. **Bordas:** NENHUM border-radius em nenhum componente. Formas retangulares reforçam estética arquitetônica.
4. **Cores:** Paleta neutra (preto, branco, cream) com toques de dourado (#C9A96E) apenas em CTAs, eyebrows e destaques.
5. **Imagens:** Todas do Unsplash, arquitetura moderna e minimalista. object-fit: cover.
6. **Hover:** Transições suaves (0.3s). Cards mudam cor da borda para dourado. Botões escurecem levemente.
7. **Scroll:** Animações fade-in-up suaves com Intersection Observer. Nada agressivo.
8. **Mobile:** Single column, hamburger menu com overlay escuro, botões full-width.
9. **Performance:** Lazy loading em imagens abaixo do fold.
10. **Navegação:** Header fixo com logo à esquerda, links ao centro, CTA à direita. Fundo transparente que fica branco ao scroll (backdrop-blur).

## IMAGENS UNSPLASH SUGERIDAS

1. **Hero:** Fachada de edifício moderno, linhas clean, céu azul — buscar "modern architecture facade minimal"
2. **Serviço 1 (Viabilidade):** Blueprints ou análise de projeto — buscar "architectural blueprints table"
3. **Serviço 2 (Urbanismo):** Vista aérea de planejamento urbano — buscar "urban planning aerial city"
4. **Serviço 3 (Arquitetura):** Edifício residencial contemporâneo — buscar "contemporary residential building"
5. **Background textures (opcional):** Concreto ou mármore sutil — buscar "concrete texture minimal"

---

## REFERÊNCIAS AWWWARDS — DIRETRIZES VISUAIS PREMIUM

> Baseado em análise de sites premiados na categoria Architecture do Awwwards.
> Documento completo: `awwwards-referencias.md`

### Sites de Referência

| Site | Nota | Destaques |
|------|------|-----------|
| **Telha Clarke** (telhaclarke.com.au) | 7.6 | Hover interativo, parallax grid, page transitions, loader animation |
| **Studio Dado** (studiodado.com) | 7.46 | Branding animation, tons terrosos (similar ao gold #C9A96E), tipografia dominante |
| **Springs** (springs.estate) | 7.23 | Gallery scroll, water animation, map interativo, luxury real estate |
| **Cargo Architecture** (cargoarchitecture.ca) | Nominee | Portfolio grid, whitespace generoso, navegação mínima |
| **Nine To Five** (9to5studio.it) | Nominee | Hero tipográfico espalhado, scroll fluido, GSAP animations |

### Padrões Awwwards a Implementar

#### 1. Hero Fullscreen (100vh)
- Hero deve ocupar toda a viewport inicial
- Text reveal cinematográfico: texto sobe com `overflow: hidden` (mask/curtain effect)
- Imagem com parallax via Framer Motion `useScroll` + `useTransform`
- Escala tipográfica ousada: heading `clamp(3rem, 6vw, 5rem)` ou maior

#### 2. Vocabulário de Animações Expandido
Não usar apenas `fadeInUp` em tudo. Variar entre:
- **Text mask reveal:** `overflow: hidden` + `translateY(100%)` → `translateY(0)` nos headings
- **Image scale-in:** imagem em container com `overflow: hidden`, scale `1.15` → `1.0` no scroll
- **Line draw:** linhas decorativas com `scaleX(0)` → `scaleX(1)` com `transform-origin: left`
- **Stagger refinado:** delays variados (0.05s-0.15s) entre elementos filhos
- **Parallax sutil:** imagens movendo a 0.5x-0.8x da velocidade do scroll
- **Counter animation:** números contando de 0 ao valor final com easing

#### 3. Micro-interações Premium
- **Botões:** pseudo-elemento `::before` com fill animation (width 0% → 100%) no hover
- **Links de navegação:** underline reveal animado (`scaleX(0)` → `scaleX(1)`)
- **Cards:** `translateY(-4px)` + sombra expandida + borda gold no hover
- **Ícones:** leve rotação ou scale (1.05) no hover do card pai
- **Custom cursor (opcional):** dot gold que escala em elementos clicáveis (desktop only)

#### 4. Loading/Intro Animation
- Overlay #1A1A1A cobrindo a tela
- Logo "LAR" aparece com fade + scale sutil
- Overlay sobe com `clipPath` ou `translateY(-100%)`
- Duração: 2-2.5s total
- Usar `AnimatePresence` do Framer Motion

#### 5. Smooth Scroll
- Adicionar `lenis` (~3KB) para scroll com inércia premium
- Alternativa: CSS `scroll-behavior: smooth` + Framer Motion scroll-linked animations

#### 6. Image Treatment
- Todas as imagens em container com `overflow: hidden`
- Scale-in reveal: imagem começa maior (scale 1.1-1.15) e ajusta no scroll
- Overlay gradiente sutil para legibilidade de texto sobre imagem
- Aspect ratios consistentes: 16:9 (landscape), 3:4 (portrait), 1:1 (cards)

#### 7. Escala Tipográfica Ousada
- Hero h1: `clamp(3rem, 6vw, 5rem)` — maior que o atual
- Section headings: `clamp(2.5rem, 5vw, 4rem)`
- Números decorativos (process steps): `clamp(4rem, 8vw, 7rem)`, opacidade 10-15%
- Letter-spacing negativo nos headings grandes: `-0.03em`

#### 8. Layout Assimétrico Intencional
- Serviços: em vez de 50/50 simétrico, usar 55/45 ou 60/40 com imagem maior
- Grid de cards: variação de tamanhos (1 card grande + 2 menores)
- Offsets verticais: elementos levemente desalinhados para dinamismo

#### 9. Elementos Decorativos Sutis
- Linhas finas (#E5E2DC) como separadores entre seções
- Linha accent (#C9A96E, 40-60px) como marcador de seção
- Números ordinais grandes e semi-transparentes ("01", "02") nos processos
- Aspas decorativas oversized nos depoimentos

#### 10. Transições entre Seções
- Fundo alternando: branco → cream → branco → dark (ritmo visual)
- Dividers animados entre seções (line draw on scroll)
- Overlap sutil: elementos da próxima seção começam a aparecer antes

### Stack Técnico (Sem Mudanças)
- **Next.js 15** (App Router, static export)
- **Tailwind CSS v4** (utility-first, design tokens via CSS variables)
- **Framer Motion** (`useScroll`, `useTransform`, `AnimatePresence`, `motion`)
- **Lucide React** (ícones line-style)
- **Opcional:** `lenis` (~3KB) para smooth scroll premium
