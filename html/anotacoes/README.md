# Anotacoes

## HTML

### Exemplo explicado

```html
  - A <!DOCTYPE html>declaração define este documento como HTML5
  - O <html>elemento é o elemento raiz de uma página HTML
  - O <head>elemento contém informações meta sobre o documento
  - O <title>elemento especifica um título para o documento
  - O <body>elemento contém o conteúdo da página visível
  - O <h1>elemento define um cabeçalho grande (sucessivamente até o 6)
  - O <p>elemento define um parágrafo
  - O <pre>elemento HTML define o texto pré-formatado (Fonte e quebra de linha)
    
Link: <a href="https://www.w3schools.com">This is a link</a>
Imagem: <img src="img_girl.jpg" width="500" height="600">
Imagem com descrição: <img src="img_girl.jpg" alt="Girl with a jacket" width="500" height="600"> ou style="width:500px;height:600px;"
Imagem com link nela: <a href="colocarolink" target="_blank">
Botões: <button>Click me</button>
Design da fonte: Cor <p style="color:red">I am a paragraph</p>
                 Tamanho <p style="font-size:50px;">I am big</p>
                 Cor de fundo <p style="background-color:powderblue;">Olaaa</p> (Cores padrão: https://www.w3schools.com/colors/colors_names.asp)
                 Fonte <p style="font-family:tahoma;">This is a paragraph.</p>
                 Alinhamento <p style="text-align:center;">Centered paragraph.</p>
                 Bordas <h1 style="border: 2px solid Tomato;">Hello World</h1>
<b> - Texto em negrito
<strong> - texto importante
<i> - texto em itálico
<em> - texto enfatizado
<mark> - texto marcado
<small> - pequeno texto
<del> - texto excluído
<ins> - texto inserido
<sub> - texto subscrito
<sup> - Texto sobrescrito

Cabeçalho maior: <h1 style="font-size:60px;">Heading 1</h1>
Escrita PT: <meta charset="UTF-8"> (Dentro do head)
Quebra de linha no mesmo paragrafo: <p>This is<br>a paragraph<br>with line breaks.</p> (br é uma tag vazia, não precisa de finalização)
Citação texto de outro site: <blockquote cite="http://www.worldwildlife.org/who/index.html"> texto aqui </blockquote>
Citação curta: <q> </q>
Abreviação: <abbr> Ex: <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
Informações de contato: <address>
Título de um trabalho/obra: <cite> Ex: <p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
Substituição bidirecional: <bdo> Ex:<bdo dir="rtl">This text will be written from right to left</bdo>
Comentários: <!-- This is a comment --> (Não aparecem no navegador, útil para encontrar erros)
    
    Attribute	Description
alt:Especifica um texto alternativo para uma imagem, quando a imagem não pode ser exibida
disabled:Especifica que um elemento de entrada deve ser desativado
href:Especifica o URL (endereço da web) de um link
id:Especifica um id exclusivo para um elemento
src:Especifica o URL (endereço da web) de uma imagem
style:Especifica um estilo CSS inline para um elemento
title:Especifica informações extras sobre um elemento (exibido como uma dica de ferramenta)
Mais descrições de atributos: https://www.w3schools.com/tags/ref_attributes.asp
    
Head é um conteiner para metadados, ele não aparece na página web, mas serve para colocar atributos.
    Ex: Title, meta, fontes e scripts
    
CSS Interno
Para a pagina toda, dentro do head:
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>

CSS Externo
Para o arquivo todo, dentro do head:
<link rel="stylesheet" href="styles.css">
Obs: Uma folha de estilos externa pode ser escrita em qualquer editor de texto. O arquivo não deve conter nenhum código HTML e deve ser salvo com uma extensão .css.
    
Borda CSS: p {border: 1px solid powderblue;}

Margem CSS p {
  border: 1px solid powderblue;
  margin: 50px;
}

Atributo ID: 
<html>
<head>
<style>
#p01 {
  color: blue;
}
</style>
</head>
<body>

<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
<p id="p01">I am different.</p>

</body>
</html>

Classe atributo:
<html>
<head>
<style>
p.error {
  color: red;
}
</style>
</head>
<body>

<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
<p class="error">I am different.</p>
<p>This is a paragraph.</p>
<p class="error">I am different too.</p>

</body>
</html>

LINKS Cores, ex:
<style>
a:link {
  color: green; 
  background-color: transparent; 
  text-decoration: none;
}

a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
}

a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}

a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}
</style>

O O targetatributo especifica onde abrir o documento vinculado.

O atributo de destino pode ter um dos seguintes valores:

_blank - abre o documento vinculado em uma nova janela ou guia
_self - Abre o documento vinculado na mesma janela / guia quando foi clicado (esse é o padrão)
_parent - Abre o documento vinculado no quadro pai
_top - Abre o documento vinculado em todo o corpo da janela
framename - abre o documento vinculado em um quadro nomeado
Ex: <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>

Foto link, ex:
<a href="linkweb">
  <img src="linkimage" alt="titulo" style="width:42px;height:42px;border:0">
</a>
