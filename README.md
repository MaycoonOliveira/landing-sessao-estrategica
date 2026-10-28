# Escala Previsível — Landing Page

Página desenvolvida para um **teste prático**, construída com **HTML5 e CSS3 puro**,
sem frameworks, bibliotecas, pré-processadores ou templates prontos.

O tema é uma **sessão estratégica gratuita** para donos de negócios digitais que
querem estruturar crescimento, processos e escala com previsibilidade.

🔗 **Deploy:** _adicione aqui a URL após publicar (Netlify / Vercel)_ 
_Ex.: https://escala-previsivel.netlify.app_

---

## ✨ Destaques

- **100% HTML + CSS puro** — zero JavaScript, zero dependências de build.
- **Tema claro/escuro** com toggle no header (técnica de checkbox + seletor `:has()`).
- **Menu lateral (drawer) no mobile** e **modal de confirmação** ao aplicar — ambos
  feitos só com CSS (seletor `:target`), sem nenhum JavaScript.
- **Responsivo de verdade** — layout fluido (mobile-first) com `clamp()` e breakpoints
  em 600px, 860px e 1040px.
- **Design premium** fiel à linguagem visual de referência: tema dark, glows azuis,
  CTAs em gradiente dourado, cards em glassmorphism e micro-interações.
- **Ilustrações e ícones em SVG** desenhados à mão (logo, favicon, gráfico do hero e
  retrato do especialista) — nada depende de imagens externas, o que torna o deploy
  totalmente autossuficiente.
- **Acessibilidade**: HTML semântico, landmarks, `skip-link`, foco visível, textos
  alternativos e suporte a `prefers-reduced-motion`.
- **Performance**: sem requisições pesadas; apenas a fonte via Google Fonts.

---

## 📁 Estrutura

```
escala-previsivel/
├── index.html          # Marcação semântica da página
├── css/
│   └── styles.css      # Design system + estilos (organizado por seções)
├── assets/
│   ├── logo.svg        # Marca (emblema de crescimento)
│   └── favicon.svg     # Ícone da aba
└── README.md
```

---

## 🧱 Seções da página

1. **Hero** — headline, subheadline, CTA principal e selos (gratuita · vagas limitadas · aplicação).
2. **Se identifica?** — dores do público em cards + destaque de contexto.
3. **O que a sessão entrega** — diagnóstico, plano de ação e visão de longo prazo.
4. **Especialista** — apresentação do mentor (personagem fictício para o teste).
5. **Como funciona** — os 4 passos da aplicação.
6. **CTA final / formulário** — aplicação com campos e disclaimer.

Todo o conteúdo textual segue a **copy base** fornecida no teste. As referências
visuais (desktop e mobile) foram usadas como inspiração de estrutura, hierarquia e
estilo — não como cópia fiel, conforme orientação das observações técnicas.

---

## ▶️ Como rodar localmente

Não há build. Basta abrir o arquivo:

```bash
# opção 1 — abrir direto
open index.html        # macOS   (no Linux: xdg-open | no Windows: start)

# opção 2 — servidor local simples (opcional)
python3 -m http.server 8080
# depois acesse http://localhost:8080
```

---

## 🚀 Deploy

A página é **estática**, então o deploy é imediato em qualquer provedor:

- **Netlify** — arraste a pasta do projeto em app.netlify.com/drop, ou conecte o
  repositório (sem build command; publish directory = raiz do projeto).
- **Vercel** — importe o repositório; framework preset **"Other"**, sem build.

---

## ⚠️ Observações técnicas

- **Imagens do especialista**: por decisão de projeto, o retrato é uma **ilustração
  vetorial (SVG)** criada sob medida, mantendo a página autossuficiente e sem
  dependências externas. Caso se queira usar uma foto real ou gerada por IA, basta
  adicioná-la em `assets/img/` e substituir o bloco `.portrait__art` no `index.html`.
- **Formulário**: é **front-end apenas** (sem back-end). A marcação já está pronta e
  acessível; para capturar os leads, basta conectar a um serviço de formulários
  (ex.: Netlify Forms, Formspree) ou a um endpoint próprio.
- **Modal de confirmação**: ao clicar em *"Quero aplicar agora"* abre um modal de
  sucesso, feito 100% em CSS. A mensagem é genérica ("Parabéns! Você acaba de se
  inscrever…") porque exibir **o nome digitado** dentro do modal exigiria JavaScript —
  o que fugiria da regra "apenas HTML e CSS puro". Caso o uso de JS seja permitido,
  a personalização com o nome é um incremento simples.
- Nenhum impedimento técnico externo afetou a entrega.
