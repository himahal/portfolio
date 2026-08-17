# 🚀 Portfólio Pessoal & UI/UX Design | Breno Pizolitto

Este repositório contém a **Versão 1.0** do portfólio profissional de **Breno Pizolitto**, refinado com um design **pixel-perfect**, arquitetura HTML5 semântica e CSS3 moderno (Flexbox, CSS Grid, Glassmorphism, Gradientes e Ícones Vetoriais SVG Inline).

---

## 📌 Visão Geral do Projeto

O portfólio tem como objetivo central apresentar o posicionamento técnico e a proposta de valor do profissional no mercado de tecnologia, destacando competências estratégicas em:

- **Automação de Processos & Web Scraping**: Desenvolvimento de robôs e scripts em Python (Selenium, Pandas) para eliminar gargalos manuais.
- **Arquitetura no Notion**: Estruturação de workspaces operacionais e gestão de processos para equipes e profissionais.
- **Inteligência Artificial Aplicada**: Integração pragmática de LLMs (Gemini API) com contexto estruturado (AI Memory) e rigor técnico (100% de auditoria e validação humana).
- **Comunicação Técnica & Treinamentos**: Tradução de conceitos complexos de engenharia para linguagem simples e acessível.

---

## 🎨 UI/UX Design System & Estética (v1.0 Pixel-Perfect)

O refinamento visual seguiu rigorosamente os arquivos de referência (`Html → Body.svg` e `Html → Body.png`), aplicando as seguintes especificações de UI/UX:

### 1. Paleta de Cores e Gradientes
- **Fundo Principal (`--bg-main`)**: `#0B1326` (Azul escuro profundo / Midnight Blue com radial glows).
- **Header Flutuante (`--bg-header`)**: `rgba(19, 27, 46, 0.85)` com efeito Glassmorphism (`backdrop-filter: blur(12px)`).
- **Cards de Conteúdo (`--bg-card-alt`)**: `#1E1B4B` (Tom índigo escuro elegante).
- **Caixas de Ícones do Toolkit (`--bg-icon-box`)**: `#171F33` com borda translúcida `#494454`.
- **Cor Primária & Destaques (`--primary` / `--primary-light`)**: `#A078FF` e `#D0BCFF`.
- **Gradiente Primário (`--primary-gradient`)**: `linear-gradient(135deg, #D0BCFF 0%, #A078FF 100%)`.
- **Tipografia (`--text-main` / `--text-muted`)**: `#DAE2FD` (Texto principal) e `#CBC3D7` (Texto secundário/suave).

### 2. Tipografia Dual
- **Títulos e Corpo**: `Plus Jakarta Sans` (pesos 400, 500, 600, 700, 800) importado via Google Fonts.
- **Botões, Métricas, Badges & Labels**: `JetBrains Mono` (pesos 400, 500, 600, 700) para visual técnico e de precisão.

### 3. Sistema de Ícones Vetoriais SVG Inline
- **Serviços Especializados**: Ícones vetoriais limpos e inline extraídos diretamente do design original em SVG:
  - *Automação Web & Desktop*: Ícone de Raio / Lightning bolt.
  - *Arquitetura no Notion*: Ícone de Equipe / Pessoas.
  - *IA Aplicada com Rigor Técnico*: Ícone de Brilho / IA Sparkles.
  - *Comunicação & Workshops*: Ícone de Chat / Comunicação.
- **Meu Toolkit**: Ícones vetoriais inline em SVG para as 8 ferramentas da grade:
  - `Python`, `Selenium`, `Pandas`, `Gemini`, `Notion`, `PowerBI`, `Linux`, `GitHub`.

---

## 🏗️ Arquitetura Técnica (HTML5 & CSS3)

A aplicação foi construída em código limpo, sem dependência de bibliotecas externas pesadas ou frameworks JavaScript:

### 1. HTML5 Semântico
- `<header class="header-container">`: Barra flutuante de navegação com logotipo, menu principal (`<nav>`, `<ul>`, `<li>`) e o botão CTA de contato.
- `<section id="hero">`: Destaque inicial com o título de impacto, descrição de valor, botões de ação, métricas numéricas e cartão de perfil com a foto (`assets/perfill.png`) com `border-radius: 24px` e badge glassmorphism sobreposta (`Diretor @ Programa Feynman (UNIVASF)`).
- `<section id="servicos">`: Apresentação dos 4 serviços em cartões interativos (`<article class="service-card">`) com ícones vetoriais SVG circulares.
- `<section id="projetos">`: Grade de exibição dos projetos em destaque (`<article class="project-card">`) com badges numéricas (`01`, `02`, `03`) e previews de imagem.
- `<section id="habilidades">`: Seção *"Meu Toolkit"* combinando uma grade 4x2 de ferramentas (`<div class="toolkit-grid">`) com o card lateral de engajamento (`<aside class="toolkit-cta-card">`).
- `<section id="contato">`: Bloco final de chamada para ação com atalho direto via `mailto`.
- `<footer>`: Rodapé semântico subdividido em navegação/links, informações de contato e direitos autorais.

### 2. Layouts Responsivos (Flexbox & CSS Grid)
- **Flexbox**: Utilizado na alinhamento do cabeçalho flutuante, agrupamento de botões, distribuição interna das métricas e estrutura do rodapé.
- **CSS Grid**:
  - `.services-grid`: Layout de 4 colunas (`repeat(4, 1fr)`).
  - `.projects-grid`: Layout de 3 colunas (`repeat(3, 1fr)`).
  - `.toolkit-container`: Grid assimétrico `1.8fr 1.2fr` unindo a grade de ferramentas e o card CTA lateral.
  - `.toolkit-grid`: Matriz 4x2 (`repeat(4, 1fr)`).

### 3. Responsividade Mobile (`@media (max-width: 768px)`)
- Adaptação do cabeçalho flutuante para coluna centralizada.
- Transição da seção Hero para layout vertical (`grid-template-columns: 1fr`).
- Reorganização automática de todas as grades bidimensionais para 1 coluna vertical sem quebras horizontais ou rolagem lateral indesejada.

---

## 📂 Estrutura de Pastas

```text
portfolio/
├── assets/
│   ├── perfill.png             # Foto de perfil otimizada do Hero (500x500 PNG)
│   ├── project-placeholder.png # Previews de projetos em alta resolução
│   ├── Html → Body.png         # Design de referência em PNG (1980x4285)
│   └── Html → Body.svg         # Design de referência em SVG original (1.8MB)
├── index.html                 # Estrutura HTML5 semântica e ícones SVG inline
├── style.css                  # Estilos CSS3 pixel-perfect, variáveis e animações
└── README.md                  # Documentação técnica completa do repositório
```

---

## 💻 Como Executar o Projeto Localmente

Como o projeto é construído em tecnologias web nativas, basta abrir o arquivo no seu navegador de preferência.

### Opção 1: Servidor HTTP Local em Python (Recomendado)

1. Abra o terminal no diretório do projeto:
   ```bash
   cd /caminho/para/portfolio
   ```

2. Execute o servidor HTTP embutido do Python 3:
   ```bash
   python3 -m http.server 8000
   ```

3. Acesse no navegador:
   ```text
   http://localhost:8000
   ```

### Opção 2: Abertura direta via `xdg-open` (Linux)

No terminal Linux, execute:
```bash
xdg-open index.html
```

---

*Desenvolvido por Breno Pizolitto.*
