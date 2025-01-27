# Capítulo 1: Introdução ao HTML

## O que é HTML?

HTML (HyperText Markup Language) é a linguagem padrão para a criação de páginas web. Ele define a estrutura de um site por meio de elementos que descrevem diferentes partes do conteúdo, como títulos, parágrafos, links, imagens e muito mais. É a base de toda a web e trabalha em conjunto com CSS (para estilização) e JavaScript (para interatividade).

---

## Principais Tags do HTML

### Estruturais

- `<html>`: Define o documento como HTML.
- `<head>`: Contém metadados sobre o documento (ex.: título, links para estilos).
- `<body>`: Abriga o conteúdo visível da página.

### Conteúdo

- `<h1>` a `<h6>`: Títulos, do mais importante (`<h1>`) ao menos importante (`<h6>`).
- `<p>`: Define um parágrafo.
- `<a>`: Cria um link.
- `<img>`: Exibe uma imagem.
- `<ul>` e `<ol>`: Listas não ordenadas e ordenadas, respectivamente.
- `<li>`: Um item de lista.

### Multimídia

- `<audio>`: Insere um áudio.
- `<video>`: Insere um vídeo.

### Formulários

- `<form>`: Define um formulário.
- `<input>`: Campo de entrada.
- `<button>`: Botão clicável.
- `<label>`: Associado a um campo de entrada.

---

## Exemplos de Uso

### Exemplo Básico de Página

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Minha Primeira Página</title>
  </head>
  <body>
    <h1>Bem-vindo ao HTML</h1>
    <p>Este é um exemplo básico de uma página HTML.</p>
    <a href="https://www.example.com">Clique aqui para saber mais</a>
    <img src="exemplo.jpg" alt="Descrição da imagem" />
  </body>
</html>
```

### Lista com Links

```html
<ul>
  <li><a href="#">Home</a></li>
  <li><a href="#">Sobre</a></li>
  <li><a href="#">Contato</a></li>
</ul>
```

### Formulário Simples

```html
<form action="/enviar" method="post">
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />

  <button type="submit">Enviar</button>
</form>
```

---

## Boas Práticas

1. **Organização e Semântica:** Utilize tags HTML semânticas (`<header>`, `<article>`, `<footer>`, etc.) para melhorar a acessibilidade e SEO.
2. **Indentação:** Indente corretamente o código para facilitar a leitura e manutenção.
3. **Atributos Alt e Title:** Sempre adicione descrições úteis para imagens e links.
4. **HTML5:** Utilize a versão mais recente do HTML para aproveitar novos recursos.
5. **Validar o Código:** Verifique seu HTML em ferramentas como o [W3C Validator](https://validator.w3.org/) para garantir conformidade com os padrões.

---

## Seção 2: Introdução ao CSS

O CSS (Cascading Style Sheets) é a linguagem utilizada para estilizar páginas web. Com ele, é possível controlar cores, espaçamentos, fontes, layouts e muitos outros aspectos visuais de um site.

### Conceitos fundamentais:

- **Seletores**: São usados para escolher os elementos HTML que serão estilizados (ex.: `div`, `.classe`, `#id`).
- **Cascata**: As regras de estilo são aplicadas com base em hierarquia e especificidade.
- **Box Model**: Todo elemento é representado como uma caixa contendo quatro partes: `content`, `padding`, `border` e `margin`.
- **Resposividade**: Permite criar designs que se adaptam a diferentes tamanhos de tela usando unidades relativas e media queries.

### Propriedades mais usadas:

1. **Cores e fundos**

   - `color`: Define a cor do texto.
   - `background-color`: Define a cor de fundo do elemento.
   - `background-image`: Aplica imagens de fundo.

   ```css
   p {
     color: #333;
     background-color: #f0f0f0;
     background-image: url("imagem.jpg");
   }
   ```

2. **Tipografia**

   - `font-family`: Define a fonte do texto.
   - `font-size`: Altera o tamanho da fonte.
   - `line-height`: Controla o espaçamento entre linhas.

   ```css
   h1 {
     font-family: "Arial", sans-serif;
     font-size: 24px;
     line-height: 1.5;
   }
   ```

3. **Tamanhos e espaçamentos**

   - `width` e `height`: Definem largura e altura.
   - `margin`: Controla o espaço externo.
   - `padding`: Controla o espaço interno.

   ```css
   div {
     width: 50%;
     height: 200px;
     margin: 20px auto;
     padding: 10px;
   }
   ```

4. **Bordas e sombras**

   - `border`: Adiciona bordas ao elemento.
   - `border-radius`: Arredonda os cantos do elemento.
   - `box-shadow`: Adiciona sombras.

   ```css
   button {
     border: 2px solid #555;
     border-radius: 8px;
     box-shadow: 2px 4px 6px rgba(0, 0, 0, 0.2);
   }
   ```

## Seção 3: Flexbox

O Flexbox é um sistema de layout unidimensional no CSS que facilita a distribuição e o alinhamento de elementos dentro de um contêiner.

### Propriedades principais:

1. **Propriedades do contêiner**

   - `display: flex`: Define o elemento como um contêiner flexível.
   - `flex-direction`: Define a direção dos itens (ex.: `row`, `column`).
   - `justify-content`: Alinha itens no eixo principal (ex.: `flex-start`, `center`, `space-between`).
   - `align-items`: Alinha itens no eixo cruzado (ex.: `stretch`, `center`, `flex-end`).
   - `flex-wrap`: Define se os itens devem quebrar para outra linha (ex.: `nowrap`, `wrap`).

   ```css
   .container {
     display: flex;
     flex-direction: row;
     justify-content: space-between;
     align-items: center;
     flex-wrap: wrap;
   }
   ```

2. **Propriedades dos itens**

   - `flex`: Controla o crescimento, encolhimento e tamanho base do item (ex.: `1 1 auto`).
   - `order`: Define a ordem dos itens.
   - `align-self`: Alinha individualmente o item no eixo cruzado.

   ```css
   .item {
     flex: 1;
     order: 2;
     align-self: flex-end;
   }
   ```

### Exemplo de aplicação:

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: stretch;
}

.item {
  flex: 1;
  padding: 10px;
  background-color: #ddd;
  margin: 5px;
}
```

## Seção 4: Grid Layout

O CSS Grid Layout é um sistema de layout bidimensional que permite criar grades complexas de maneira simples.

### Conceitos principais:

- **Contêiner de grade**: Elemento que define a grade (ex.: `display: grid`).
- **Linhas e colunas**: A grade é composta por linhas e colunas, controladas por fracionamento, tamanhos fixos ou automáticos.
- **Células**: São os espaços ocupados por um ou mais elementos na grade.

### Propriedades principais:

1. **Propriedades do contêiner**

   - `display: grid`: Define o contêiner como uma grade.
   - `grid-template-rows` e `grid-template-columns`: Define o tamanho das linhas e colunas.
   - `gap`: Controla o espaço entre as células (ex.: `row-gap`, `column-gap`).
   - `grid-template-areas`: Permite nomear áreas da grade.

   ```css
   .grid-container {
     display: grid;
     grid-template-columns: repeat(3, 1fr);
     grid-template-rows: 100px auto;
     gap: 10px;
   }
   ```

2. **Propriedades dos itens**

   - `grid-column` e `grid-row`: Define a posição do item na grade.
   - `grid-area`: Aloca o item em uma área nomeada.

   ```css
   .item {
     grid-column: 1 / 3;
     grid-row: 2 / 3;
   }
   ```

### Exemplo de aplicação:

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  grid-template-rows: 100px auto;
  gap: 20px;
}

.grid-item {
  background-color: #ddd;
  padding: 10px;
  text-align: center;
}
```

No próximo capítulo, aprenderemos sobre CSS e como ele trabalha em conjunto com o HTML para criar páginas visualmente atraentes.
