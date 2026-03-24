# Agência Criativa Web — Refatoração CSS

Projeto acadêmico de uma página responsiva para a **Agência Criativa Web**, refatorado com foco em **organização do CSS**, **padronização com metodologia BEM**, **reutilização de classes** e **facilidade de manutenção**.

## Visão geral

Esta versão foi reorganizada a partir do projeto original, com separação entre:

- `index.html` → estrutura semântica da página
- `layout.css` → regras de layout, containers, grid, flexbox e responsividade
- `style.css` → identidade visual, tipografia, botões, cards e componentes

O objetivo foi deixar o código mais limpo, modular e sustentável.

---

## Tecnologias utilizadas

- HTML5
- CSS3
- Flexbox
- CSS Grid
- Media Queries
- Unidades relativas (`rem`, `vh`, `%`, `fr`)
- Metodologia BEM

---

## Estrutura do projeto

```bash
agencia-criativa-web-refatorado/
├── index.html
├── layout.css
├── style.css
└── README.md
```

---

## Seções da página

A página contém as seguintes áreas:

- **Home** — banner principal com destaque da agência
- **Sobre nós** — descrição da proposta e valores
- **Serviços** — cards com os serviços oferecidos
- **Depoimentos** — comentários fictícios de clientes
- **Contato** — informações e formulário de contato

---

## Melhorias aplicadas na refatoração

### 1. Organização do CSS
- remoção de repetições desnecessárias
- separação entre estrutura e aparência
- hierarquia mais clara entre estilos globais e componentes

### 2. Padronização com BEM
Exemplos usados no projeto:

- `.site-header__content`
- `.section-heading__title`
- `.service-card--featured`
- `.contact-form__input--textarea`

Isso facilita leitura, manutenção e expansão futura do código.

### 3. Reutilização de classes
Foram criadas classes reutilizáveis como:

- `.container`
- `.section`
- `.card`
- `.card--light`
- `.card--dark`
- `.btn`
- `.btn--primary`
- `.btn--secondary`

### 4. Responsividade mantida
O projeto continua totalmente responsivo com:

- Flexbox no cabeçalho, botões e depoimentos
- CSS Grid nas áreas principais e na seção de serviços
- Media queries para tablets e celulares
- imagens com `srcset`

## Objetivo da atividade

Aplicar os conceitos do módulo em uma página realista, com atenção a:

- design responsivo
- manutenção de código
- organização do CSS
- nomenclatura consistente
- boas práticas de desenvolvimento front-end

---

## Autor

Projeto desenvolvido para fins acadêmicos por **Felipe Gabriel Lambiazzi**.
