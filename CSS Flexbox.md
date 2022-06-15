# CSS Flexbox

Projetado como um modelo de layout unidimensional

- **Flez container** é a tag que envolve os itens, será nela que iremos aplicar a propriedade "display:flex". Transforma todos os seu itens filhos em flex itens.
  - Pode ser aplicado em qualquer tipo de tag;
  - Propriedades relacionadas:
    - Display 
    - Flex-direction
    - Flex-wrap
    - Flex-flow
    - Justify-content
    - Align-items
    - Align-content

- **Flex item** são os elementos filhos diretos do flex container. E também podem se tornar flex container.
  - Propriedades relacionadas:
    - flex-grow
    - flex-basis
    - flex-shrink
    - flex 
    - order
    - align-self

## Flex container 

- **Display Flex** torna a tag um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos desta tag, tornam-se em flex item.

## Flex direction 

- É a propriedade que estabelece o eixo principal do container definindo assim a direção que os flex items são colocado no flex container 
  - **row** (padrão): direção do texto, esquerda para a direita;
  - **row-reverse**: sentido oposto à direção do texto;
  - **column**: ordenação de cima para baixo, em coluna unica;
  - **column-reverse**: ordenação inversa, de baixo para cima;

## Flex wrap

- É a propriedade que define se os itens devem ou não quebrar a linha;
  - Por padrão eles não quebram linhas, isso faz com que os flex itens sejam compactados além do limite do conteúdo;

- **nowrap** é o padrão, não permite a quebra de linha;
- **wrap** permite a quebra de linha assim que um dos flex itens não puder mais ser compactado;
- **wrap-reverse** permite a quebra de linha assim que um dos flex itens não puder mais ser compactado, porém na direção contrária da linha, acima;

## Flex flow

- É um atalho para as propriedade **flex-direction** e **flex-wrap**;
  - Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para colimn, mantemos o padrão de flex-wrap que é nowrap;

## Justify content

- Essa propriedade vai se encarregar de alinhar os item dentro do container de acordo com a direção pretendida a tratar da distribuição de espaçamento entre eles;
  - **OBS:** caso seus itens estejam ocupando 100% de todo o container ela não se aplica;

- **flex-start**: inícia do container;
- **flex-end**: final do container;
- **center**: ao centro do container;
- **space-between**: cria um espaçamento igual entre os elementos;
- **space-around**: os espaçamentos do meio são duas vezes maiores que o inicial e final;

## Align items

- Trata do alinhamento dos flex itens de acordo com o eixo do container;

- O alinhamento é direfente para quando os itens estão em colunas ou linhas; 

  - Permite o alinhamento central no eixo vertical;

  - Não precisa ter conhecimento da altura dos itens;

- **center**: alinhamento dos itens ao centro;
- **stretch**: padrão, e os flex itens cresçam igualmente;
- **flex-start**: alinhamento dos itens no início;
- **flex-end**: alinhamento dos itens no final;
- **baseline**: alinhamento de acordo com a linha base da tipografia dos itens;

## Align content

- É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container;
- **Precisamos** **que**:
  - O container utilize quebra de linhas;
  - A altura do container seja maior que soma das linhas dos itens;

- **Tipos de alinhamento**:
  - **Center**: alinhamento dos itens ao centro;
  - **Stretch**: é o padrão e os flex itens crescem igualmente;
  - **Flex-start**: alinhamento dos itens no início;
  - **Flex-end**: alinhamento dos itens no final;
  - **Space-between**: cria um espaçamento igual entre os elementos;
  - **Space-around**: os espaçamentos do meio são duas vezes maiores que o inicial e final;