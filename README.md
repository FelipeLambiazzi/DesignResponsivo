# 🎨 Agência Criativa Web

Projeto desenvolvido com foco em **design responsivo moderno** e **refatoração de CSS utilizando SASS**, aplicando boas práticas de organização, escalabilidade e reutilização de código.

---

## 🚀 Sobre o Projeto

A **Agência Criativa Web** é uma landing page institucional que apresenta serviços de design digital, branding e presença online.

O projeto foi inicialmente construído com CSS tradicional e posteriormente **refatorado para SASS**, visando melhorar a estrutura, manutenção e qualidade do código.

---

## 🧠 Principais Objetivos da Refatoração

* Organizar o CSS em uma arquitetura escalável
* Reduzir repetição de código
* Facilitar manutenção futura
* Aplicar boas práticas de mercado (BEM + SASS)

---

## 🛠️ Tecnologias Utilizadas

* HTML5
* CSS3
* SASS (SCSS)
* Node.js (para compilação)

---

## 📂 Estrutura do Projeto

```bash
📦 DesignResponsivo
├── 📁 css
│   └── estilos.css (arquivo compilado)
├── 📁 scss
│   ├── _base.scss
│   ├── _variaveis.scss
│   ├── _mixins.scss
│   ├── _layout.scss
│   ├── _componentes.scss
│   └── estilos.scss (arquivo principal)
├── index.html
├── package.json
└── README.md
```

---

## 🎯 Destaques da Refatoração

### ✅ 1. Organização com Partials (Arquitetura Modular)

O código foi dividido por responsabilidade:

* `_variaveis.scss` → cores, espaçamentos, fontes
* `_mixins.scss` → reutilização de estilos
* `_base.scss` → reset e estilos globais
* `_layout.scss` → estrutura da página (grid, header, seções)
* `_componentes.scss` → botões, cards, menus

👉 Resultado: código mais limpo e fácil de manter.

---

### 🎨 2. Uso de Variáveis

Padronização completa de:

* cores
* espaçamentos
* tipografia
* bordas e sombras

```scss
$color-accent: #61dafb;
$space-md: 1rem;
```

👉 Facilita manutenção e consistência visual.

---

### 🔁 3. Mixins Reutilizáveis

Criação de mixins para evitar repetição:

* botões
* cards
* inputs
* responsividade

```scss
@mixin button-base($bg, $color) {
  padding: 0.85rem 1.45rem;
  border-radius: 999px;
  background: $bg;
  color: $color;
}
```

👉 Código mais enxuto e reutilizável.

---

### 🧩 4. Metodologia BEM

Uso consistente de nomenclatura:

```scss
.nav__list
.hero__title
.card--dark
```

👉 Melhor leitura e organização dos componentes.

---

### 🌳 5. Aninhamento Controlado

Uso de nesting para manter contexto sem exagero:

```scss
.nav {
  &__link {
    &:hover {
      color: $color-accent;
    }
  }
}
```

👉 Código mais legível e estruturado.

---

### 📱 6. Responsividade Organizada

Uso de mixins para media queries:

```scss
@include respond(md) {
  .nav__list {
    flex-direction: column;
  }
}
```

👉 Melhor controle de layout em diferentes telas.

---

### ⚙️ 7. Compilação com Node.js

O projeto utiliza SASS via linha de comando:

```bash
npm install
npx sass scss/estilos.scss css/estilos.css
```

Modo watch:

```bash
npx sass --watch scss/estilos.scss:css/estilos.css
```

---

## 💡 Principais Aprendizados

* Organização de CSS em projetos reais
* Uso de arquitetura modular com SASS
* Aplicação prática da metodologia BEM
* Separação entre estrutura (layout) e componentes
* Escrita de código mais escalável e profissional

---

## 🔥 Diferenciais do Projeto

* Refatoração completa de CSS tradicional para SASS
* Estrutura pronta para crescimento do projeto
* Código limpo, reutilizável e bem organizado
* Foco em boas práticas utilizadas no mercado

---

## 📸 Preview

> Interface moderna, responsiva e com foco em experiência do usuário.

---

## 👨‍💻 Autor

**Felipe Gabriel Lambiazzi**

* 💼 Desenvolvedor em formação
* 🔗 [LinkedIn](https://www.linkedin.com/in/felipe-gabriel-lambiazzi-734861140/)
* 📧 [felipelambiazzi17@gmail.com](mailto:felipelambiazzi17@gmail.com)

---

## 📌 Considerações Finais

Este projeto representa a transição de um código simples para uma estrutura profissional, demonstrando evolução técnica e preocupação com qualidade e escalabilidade.

---

⭐ Se você gostou do projeto, não esqueça de deixar uma estrela!
