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

No próximo capítulo, aprenderemos sobre CSS e como ele trabalha em conjunto com o HTML para criar páginas visualmente atraentes.
