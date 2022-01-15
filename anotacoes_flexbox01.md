# JAVASCRIPT_FLEXBOX
ANOTACÕES GERAIS SOBRE CSS / HTML 

# FLEXBOX.

# Aplicando flex-direction

<style>
      .flex-container {
        margin: 0;
        padding: 0;
        display: flex;
        list-style: none;
      }


      .item {
        background-color: darkblue;
        height: 50px;
        width: 50px;
        line-height: 50px;
        color: white;
        font-size: 20px;
        text-align: center;
        margin: 4px;
      }
      .row {
        flex-direction: row;
      }
      .row-reverse {
        flex-direction: row-reverse;
      }
      .row-reverse li {
        background-color: crimson;
      }
      .column {
        float: left;
        flex-direction: column;
      }
      .column li {
        background-color: cyan;
      }
      .column-reverse {
        float: right;
        flex-direction: column-reverse;
      }
      .column-reverse li {
        background-color: darkgreen;
      }
    </style>

  </head>
  <body>
    <p>flex container</p>
    <ul class="flex-container row">
      <li class="item">1</li>
      <li class="item">2</li>
      <li class="item">3</li>
      <li class="item">4</li>
    </ul>

    <ul class="flex-container row-reverse">
      <li class="item">1</li>
      <li class="item">2</li>
      <li class="item">3</li>
      <li class="item">4</li>
    </ul>
    
    <ul class="flex-container column">
      <li class="item">1</li>
      <li class="item">2</li>
      <li class="item">3</li>
      <li class="item">4</li>
    </ul>
    
    <ul class="flex-container column-reverse">
      <li class="item">1</li>
      <li class="item">2</li>
      <li class="item">3</li>
      <li class="item">4</li>
    </ul>

  </body>
</html>

# Aplicando flex-wrap

(é a propriedade que define se os itens deven ou não quebrar linha)
\*por padrão eles não quebram linhas , isso faz com que os flex itens sejam
compactdos além do limite do conteúdo. \* (NOWWRAP) é o padrão , não quebra de linha.
\*(WRAP) permite a quebra de linha assim que um dos flex itens não puder mais ser compactado.

# Flex-flow

\* é um atalho para as propriedades flex-direction e flex-wrap
porém seu uso não é tão comum , visto que , quando mudamos o flex-direction para column,
mantemos o padrão do flex-wrap que é nowwrap(linhas não quebra)

# Justify Content

/\* essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.
obs... caso seus itens esteja ocupando 100% de todo o container, ele nã se aplica.
/\* Variações
. flex-start: inicio do container
. flex-end: final do container
. center : ao centro do container
. space-between: cria um espaçamento igual entre os elementos
. space-around : os espaçamentos do meio são duas vezes maiores que o inicial e o final.

# Aligment-Items

\*trata do alinhamento dos flex itens de acordo com o eixo do container \* O alimhanmento é diferente para quando os itens estão em colunas ou linhas \* permite o alinhamento central no eixo vertical

/\*tipos de alinhamentos

- center: alinhamento dos itens ao centro
- strech: padrão , e os flex itens cresçam igualmente
- flex-start: alinhamento dos itens no inicio
- flex-end: alinhamento dos itens no final
- baseline: alinhamento de acordo com a linha base da tipografia dos itens

# Align-content (eixo vertical)

\* é a propriedade responsavel por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.

- O container utilize quebra de linhas
- a altura do container seja maior que a soma das linhas dos itens

\* tipos de alinhamento

- center : alinhamento dos itens ao centro
- strech: é o padrão e os flex itens crescem igualmente .
- flex-start:alinhamento dos itens no inicio
- flex-end:alinhamento dos itens no final
- space-between:cria um espaçamento igual entre os elementos
- space-around:os espaçamentos do meio são duas vezes maiores que o inicial e final.

# FLEX-GROW (trabalha só com numeros)

\* define a proporcionalidade de crescimento dos itens , respeitando o tamanho de seus conteúdos internos.
obs. não irá funcionar caso tenhamos adicionado justify-content ao nosso flex-container.

# FLEX-BASIS

\* É a propriedade que estabelece o tamanho inicial do item antes das distribuições de espaço restante dentro dele, usando como base o conteúdo interno disposto.
-valores possiveis
-auto:caso o item não tenha tamanho,este será proporcional ao conteúdo do item
-px,%,em....: são valores exatos previamente definidos
-(zer0):terá relação com a definição do flex-grow.

# FLEX-SHRINK (redução do tamanho)

\* é a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.

# FLEX

\* esta propriedade é um atalho ou abreviação de escrita para as propriedades:grow, shrink e basis.

# ORDER
