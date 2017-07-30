# Entendendo o Document Object Model (DOM)

Percebo que o DOM é um assunto extremamente importante mas nem tanto abordado, entender como realmente funciona nossos navegadores ajuda muito na compreensão de diversos outros assuntos.


Criado pelo W3C, o **Document Object Model** ou simplesmente **DOM** representa como as marcações em HTML e XML são organizadas e lidas pelo navegador que você usa.


O DOM representa os objetos de uma página em forma de uma árvore e pode ser modificada com uma linguagem de script, como o JavaScript.


## Entendendo um pouco melhor

Quando uma página da web é carregado ela se torna um **document object**, esse document object é a raiz do nosso documento e pai de todos outros elementos da página.

O **DOM** é a interface para os scripts (javascript) se comunicarem com os objetos/elementos do HTML.

Vamos a um exemplo de código HTML: 


```HTML
<!DOCTYPE html>
<html>
    <head>
        <title>Exemplo de Documento</title>
    </head>
    <body>
        <h1>Este é um documento HTML</h1>
        <p>Este é um <i>simples</i> documento</p>
    </body>
</html>
```


**Essa é a representação visual DOM do código acima e como ele é reconhecido pelos navegadores**

![Cah Felix](/imgs/dom.jpg?style=centerme)

**Detalhando um pouquinho mais essa árvore**

![Cah Felix](/imgs/dom-no.jpg?style=centerme)


Em nosso exemplo de árvore DOM temos 3 tipo de nó:


### Nó de Elemento (Element Nodes)

Pode ter filhos e/ou atributos;

Exemplo: tags HTML



### Nó de texto (Text nodes)

Guarda basicamente texto puro, que pode ser renderizado ou trabalhado via script

Não pode ter filhos

Exemplo: texto de um elemento 



### Nó de atributo (Attribute nodes)

Os atributos são propriedades do elemento, não filhos do elemento. Essa distinção é importante por causa dos métodos usados para navegar no DOM

Exemplo: o href

## Concluindo

O propósito desse post foi apresentar o DOM, resumidamente DOM é uma representação de uma página html no mundo javascript e pode ser acessado a partir da variável document, que representa a raiz de nossa página, permitindo manipular o DOM (não o HTML, pois nao mexemos no arquivo.html). Alteramos classes, textos, criamos elementos, etc.


## Artigos anteriores
[Início](https://github.com/cahfelix/artigos-react)

[1 - Entendendo o React](entendendo-o-react.md)

[2 - Linha do tempo para aprendizagem do react](linha-do-tempo-da-aprendizagem-do-react.md)



