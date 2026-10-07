# Stark Industries — Mark LXXXV

Página conceito inspirada no Homem de Ferro: o usuário "roda um diagnóstico" da armadura Mark LXXXV rolando a página. Uma sequência de 169 quadros é desenhada em canvas e avança conforme o scroll, com falas do Tony Stark aparecendo em pontos específicos da animação.

🔗 **Ao vivo:** [iron-man-dusky.vercel.app](https://iron-man-dusky.vercel.app)

> Projeto de fã, sem fins comerciais e sem vínculo com a Marvel ou a Disney. Feito para estudo e portfólio.

## Stack

Next.js (App Router) · React · TypeScript · Tailwind CSS 4 · Framer Motion · Lenis · ESLint

## Destaques

- **Sequência de frames em canvas:** 169 imagens pré-carregadas e desenhadas com `drawImage`, sincronizadas à posição do scroll
- **Diálogos por progresso:** cada fala tem janela de entrada e saída definida em dados (`src/lib/hero.ts`), separando conteúdo de animação
- Interface estilo HUD (telemetria, moldura, contador de sequência) com componentes reutilizáveis
- Smooth scroll com Lenis via provider; reveals com Framer Motion

## Estrutura

```
src/app/                         layout e página
src/components/sections/         Hero, CinematicReveal, SystemsNominal, Footer
src/components/ui/               HudFrame, Navbar, AnimatedSection, EyebrowBadge
src/components/providers/        SmoothScrollProvider (Lenis)
src/lib/                         dados da sequência e dos diálogos
```

## Rodar localmente

```bash
npm install
npm run dev     # http://localhost:3000
```

---

Design e código: **Whallyson Gabriel** · [Portfólio](https://whallyson-of-web.vercel.app) · [LinkedIn](https://www.linkedin.com/in/whallyson-gabriel-garcia-da-silva-914765235)
