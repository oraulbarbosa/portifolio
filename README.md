# Portfólio Pessoal — Raul Henrique Barbosa

<img src="img/tela inicial site.png" alt="tela inicial">

![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?logo=bootstrap&logoColor=white)

## Nome do aluno

**Raul Henrique Barbosa**

## Descrição do portfólio

Portfólio pessoal desenvolvido para apresentar meu perfil profissional, minhas
habilidades técnicas, os projetos que venho construindo e as formas de contato.

O design segue uma estética **minimalista em preto e branco**, com tipografia
monoespaçada (JetBrains Mono) nos elementos de destaque — a mesma identidade
visual da versão inicial do projeto, agora evoluída com novas seções e recursos
interativos.

O site é dividido em:

- **Hero** — apresentação inicial com foto de perfil
- **Sobre mim** — trajetória e objetivos
- **Habilidades** — grade de ícones das tecnologias que uso
- **Projetos** — carousel + cards com os projetos publicados
- **Contato** — e-mail, GitHub e LinkedIn
- **Footer** — créditos

## Tecnologias utilizadas

| Tecnologia | Uso no projeto |
|---|---|
| **HTML5** | Estrutura semântica das seções |
| **CSS3** | Variáveis CSS, grid, keyframes, transições |
| **Bootstrap 5** | Navbar, grid, cards, carousel, utilitários |
| **Bootstrap Icons** | Ícones de habilidades e contato |
| **Google Fonts (JetBrains Mono)** | Tipografia dos destaques |

## Link do site publicado

👉 **[https://oraulbarbosa.github.io/portfolio](https://oraulbarbosa.github.io/portifolio/)/**

## Explicação do funcionamento do projeto

A navegação é feita por uma **navbar Bootstrap fixa** no topo da página, com
menu hambúrguer automático em telas pequenas. Os links usam âncoras
(`#sobre`, `#habilidades`, `#projetos`, `#contato`) com rolagem suave via
`scroll-behavior: smooth` e `scroll-padding-top` para compensar a altura da
navbar.

Todo o layout usa o **sistema de grid do Bootstrap**, garantindo adaptação
automática a celular, tablet e desktop.

A seção de **Projetos** combina um **carousel** (destaque visual) com **cards**
abaixo (leitura confortável em telas pequenas).

As cores e fontes são definidas em variáveis CSS no `:root`, mantendo
consistência em todo o site. Todos os efeitos de hover (cards, foto, ícones,
links) são feitos em **CSS puro** com `transition` e `transform`.

## Recurso novo adicionado

Foram adicionados **dois recursos novos** além do que foi construído em aula,
ambos com **Bootstrap + CSS puro**, sem JavaScript customizado:

### 1. Seção de Habilidades com ícones interativos
Uma seção nova apresenta 7 tecnologias (HTML5, CSS3, Bootstrap, Python, Git,
GitHub e Design) apenas com **ícones do Bootstrap Icons** e o nome
abaixo. Nada de porcentagens ou barras — mantendo o estilo minimalista da
versão antiga.

### 2. Carousel do Bootstrap na seção Projetos
Os 3 projetos são apresentados em um **carousel nativo do Bootstrap** com
indicadores, botões prev/next e legendas, dando destaque visual aos trabalhos.

## Como o recurso novo foi implementado

### Habilidades (ícones)
A seção usa uma **grade CSS responsiva** criada com `display: grid`,
`grid-template-columns: repeat(auto-fill, minmax(120px, 1fr))` e `gap`. Cada
habilidade é um card com um ícone do Bootstrap Icons (`<i class="bi ...">`) e
um `<span>` com o nome da tecnologia. O hover reutiliza o mesmo padrão de
interação dos cards de projeto (leve elevação com `transform` e mudança de
borda/fundo via `transition`). Tudo em **HTML e CSS puros**, sem JavaScript.

### Carousel dos projetos
Uso do componente **nativo do Bootstrap 5** (`carousel`, `carousel-indicators`,
`carousel-inner`, `carousel-item`, `carousel-control-prev` e
`carousel-control-next`). A navegação automática e os botões são ativados
pelos atributos `data-bs-ride`, `data-bs-slide` e `data-bs-target`. A altura
das imagens foi padronizada em 420px via CSS para manter a consistência
visual. Nenhum JavaScript foi escrito manualmente — apenas o bundle do
Bootstrap (via CDN) é usado para ativar o componente.

## Estrutura do repositório

```
📦 portfolio
 ┣ 📂 img
 ┃ ┣ perfil.jpg
 ┃ ┣ entretenimento.jpg
 ┃ ┣ avaliacap.jpg
 ┃ ┗ agua.jpg
 ┣ 📄 index.html
 ┗ 📄 README.md
```


## Como executar localmente

1. Clone o repositório:
   `git clone [https://github.com/oraulbarbosa/portfolio.git](https://github.com/oraulbarbosa/portifolio.git)`
2. Abra o arquivo `index.html` no navegador (ou use a extensão Live Server do VS Code).

Não há dependências para instalar — tudo via CDN.

## Publicação no GitHub Pages

1. Acesse o repositório no GitHub
2. Vá em **Settings → Pages**
3. Em *Source*, selecione **Deploy from a branch**
4. Escolha a branch **main** e a pasta **/ (root)**
5. Salve e aguarde alguns segundos — o site estará em
   `[https://oraulbarbosa.github.io/portfolio/](https://oraulbarbosa.github.io/portifolio/)`

## Contato

- **E-mail:** raulbarbosa.dev@gmail.com
- **GitHub:** https://github.com/oraulbarbosa
- **LinkedIn:** https://www.linkedin.com/in/raul-henrique-barbosa-92b13a6a/

---

© 2025 Raul Henrique Barbosa — Desenvolvido com HTML, CSS & Bootstrap.
