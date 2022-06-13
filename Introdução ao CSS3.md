# Introdução ao CSS3

- Seletores: a, p, h1, h3 {

  color: blue;

  font-size: 14px; (Declarações)

  }

## ID x Classe 

- < header id="header" class="header"></ header>
- < header class="header"></ header>
- Representa qualquer tipo de elemento
- classe é preterido por um ponto 
- um id é preterido por uma hash (id só pode ser usado uma vez na página)

## Box model 

- Margin: Espaçamento entre os elementos;
- Border: Circundam o padding e o conteúdo (podemos alterar largura e cor);
- Padding: Espaçamento entre a borda e o conteúdo;
- Content: O que o bloco representa;

## Estilizando elementos 

### Padding e Margin

- Colocando um valor para a parte superior e inferior;

- .post {

  padding: 15px, 10px, 5px, 0;

  }

  - Superior, direita, baixo e esquerda;

- .post {

  padding-top: 15px;

  padding-right: 10px;

  padding-bottom: 5px;

  padding-left: 0;

  }

  - Usado quando nós temos um padding ou margin com 3 lados iguais e um só diferente.

### Background

- .post {

​		background-color: green;

​		background-image: url("bg.png");

​		background-position: top;

​		}

- [MDN](https://developer.mozilla.org/pt-BR/) Estudar CSS

### Border

- Largura: pixels, centímetros, milímetros...

- Cor: blue, #0000ff

- Estilo: sólida, pontilhada, tracejada...

  .post{

  border: 3px solid blue;

  border-top: 2px dotted green;

  border-right: 4px dashed pink;

  }

#### Border-radius (Arredonda as bordas)

- Border-radius: 10px;
- Border-radius: 50%;
- Border-radius:10% 20%;
- Border-radius:10% 20% 15% 22%;

- Topo, direita, inferior, esquerda;

## Estilizando textos 

- **font-family** altera a fonte do texto;

  - #title{

    font-family: Verdana;

    }

  - .post_title{

    font-family: Verdana, Arial;

    }

- **font-size** altera o tamanho do texto;

  - #title{

    font-size: 30px;

    }

  - .post_title{

    font-size: 18px;

    }

- **font-style** altera a aparência do texto;

  - #title {

    font-style: normal;

    }

  - .subtitle {

    font-style: italic;

    }

- **font-weight** altera peso do texto

  - #title {

    font-weight: normal;

    }

  - .subtitle {

    font-weight: bold;

    }

- **text-transform** alterna o texto entre maiúsculas e minúsculas;

  - #title {

    text-trasnform: uppercase;   (Maiúsculo)

    }

  - .subtitle {

    text-transforma: lowercase;      (minúsculo)

    }

  - .post_title {

    text-transform: capitalize;      (primeira letra maiúscula)

    }

- **text-decoration** dar destaque a um texto;

  - #title {

    text-decoration: underline;

    }

  - .subtitle {

    text-decoration: overline;

    }

  - .post_title{

    text-decoration: line-through;

    }

## Estilizando listas

- **list-style-type** 

  - ul {

    list-style-type: square;

    }

  - ol {

    list-style-type: upper-roman;

    }

  - ul {

    list-style-type: "\1F44D";

    }

  - ul {

    list-style-image: url("rocket.png");

    }

## Dimensão e alinhamento 

- Width ajustar a largura;

- Height ajustar a altura;

  

- Max-width largura máxima

- Max-height altura máxima

  

- Margin espaçamento entre elementos

  

- Text align alinhar textos