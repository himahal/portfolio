# 🚀 Portfólio Pessoal | Breno Pizolitto

Este repositório contém a **Versão 1.0** do portfólio profissional de **Breno Pizolitto**, desenvolvido com foco em arquitetura semântica, design moderno e alta performance visual/estrutural.

---

## 📌 Sobre o Projeto

O portfólio tem como objetivo central apresentar o posicionamento técnico e a proposta de valor do profissional no mercado de tecnologia, destacando competências estratégicas em:

- **Automação de Processos & Web Scraping**: Desenvolvimento de robôs e scripts em Python (Selenium, Pandas) para eliminar gargalos manuais.
- **Arquitetura no Notion**: Estruturação de workspaces operacionais e gestão de processos para equipes e profissionais.
- **Inteligência Artificial Aplicada**: Integração pragmática de LLMs (Gemini API) com contexto estruturado (AI Memory) e rigor técnico (100% de auditoria e validação humana).
- **Comunicação Técnica & Treinamentos**: Tradução de conceitos complexos de engenharia para linguagem acessível.

---

## 🏗️ Arquitetura Atual (v1.0)

A versão v1.0 foi construída utilizando puramente **HTML5 Semântico** e **CSS3 Moderno**, sem dependência de frameworks externos ou bibliotecas pesadas.

### 1. HTML5 Semântico (Mapeamento de Seções)
O documento `index.html` foi estruturado para garantir acessibilidade, otimização SEO e legibilidade do código:

- `<header>`: Barra de navegação fixa contendo logotipo, menu principal de links (`<nav>`, `<ul>`, `<li>`) e o botão principal de call-to-action (CTA).
- `<section id="hero">`: Seção de destaque inicial com título de impacto, resumo de posicionamento, métricas numéricas (`4+ anos na Cactus Rockets`, `100% de Auditoria Humana`), botões de ação e imagem de perfil otimizada.
- `<section id="servicos">`: Apresentação dos 4 pilares de atuação através de cartões reutilizáveis (`<article class="service-card">`).
- `<section id="projetos">`: Grade de exibição dos projetos em destaque (`<article class="project-card">`) com imagens de preview, títulos e direcionamento externo.
- `<section id="habilidades">`: Seção *"Meu Toolkit"* que combina a grade de tecnologias com um cartão de destaque lateral (`<aside class="toolkit-cta-card">`) para conversão.
- `<section id="contato">`: Bloco final de engajamento (CTA) com atalho direto via `mailto`.
- `<footer>`: Rodapé semântico subdividido em `.footer-top` (links de navegação, política de privacidade e redes sociais) e `.footer-bottom` (direitos autorais).

### 2. CSS3 Modular & Design System
O arquivo `style.css` adota boas práticas de arquitetura de estilos:

- **Design Tokens (`:root`)**: Centralização das variáveis de cores e efeitos para manter consistência em toda a aplicação:
  ```css
  :root {
      --bg-main: #0a0e17;
      --bg-card: #131a2a;
      --bg-card-hover: #1b2438;
      --primary: #9d7bf5;
      --primary-glow: rgba(157, 123, 245, 0.2);
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
      --border-color: rgba(255, 255, 255, 0.08);
  }
  ```
- **Reset Global**: Higienização das margens, preenchimentos e padronização do modelo de caixa (`box-sizing: border-box`).
- **Flexbox 1D**: Empregado para layouts unidimensionais (alinhamento do cabeçalho, distribuição de botões, cartões de serviços e estrutura interna do rodapé).
- **CSS Grid 2D**: Empregado na organização de componentes bidimensionais complexos:
  - `.services-grid`: Layout de 4 colunas (`repeat(4, 1fr)`).
  - `.projects-grid`: Layout de 3 colunas (`repeat(3, 1fr)`).
  - `.toolkit-container`: Layout assimétrico dividindo a grade de ferramentas (`2fr`) e o card lateral (`1fr`).
  - `.toolkit-grid`: Matriz 4x2 para ícones/tecnologias (`repeat(4, 1fr)`).

### 3. Estratégia de Responsividade
A adaptação para dispositivos móveis e tablets adota um breakpoint fluido em `@media (max-width: 768px)`:
- **Hero Section**: Transição de layout horizontal para `flex-direction: column-reverse` (destacando a foto no topo e o texto abaixo).
- **Grids Fluidas**: Colapso automático de todas as grades bidimensionais (`.services-grid`, `.projects-grid`, `.toolkit-container`, `.toolkit-grid`) para coluna única (`grid-template-columns: 1fr`).

---

## 📂 Estrutura de Pastas

```text
portfolio/
├── assets/
│   ├── file_pixian_ai.png     # Imagem de perfil do Hero
│   └── project-placeholder.png # Previews dos projetos
├── index.html                 # Estrutura HTML5 semântica
├── style.css                  # Folha de estilos CSS3 modular
└── README.md                  # Documentação técnica do repositório
```

---

## 🗺️ Roadmap de Evolução

- [x] **v1.0 (Atual)**: Portfólio estático semântico, responsivo, estruturado com HTML5 puro e CSS3 moderno.
- [ ] **v2.0**: Introdução de interatividade dinâmica via JavaScript nativo (ES6+), manipulação de DOM, filtros de projetos e catálogo dinâmico de templates/cursos.
- [ ] **v3.0**: Arquitetura Fullstack com backend em Node.js / Express, integração de APIs RESTful (consumo de dados do GitHub e Gemini API), armazenamento em banco de dados e autenticação de usuários.

---

## 💻 Como Executar o Projeto (Linux)

Como o projeto v1.0 utiliza apenas tecnologias nativas do navegador, não é necessária a instalação de dependências `npm`.

### Opção 1: Servidor HTTP local via Python (Recomendado)

1. Abra o terminal na raiz do projeto:
   ```bash
   cd /caminho/para/portfolio
   ```

2. Inicie o servidor embutido do Python 3:
   ```bash
   python3 -m http.server 8000
   ```

3. Abra o navegador e acesse:
   ```text
   http://localhost:8000
   ```

### Opção 2: Abertura direta via `xdg-open`

No terminal Linux, execute:
```bash
xdg-open index.html
```

---

*Desenvolvido por Breno Pizolitto.*
