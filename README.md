# Curso_BootStrap5
Curso do framework BootStrap5. O mesmo foi ministrado pelo prof. Ricardo Maroquio.

---

Até o presente momento, foi estudado os conceitos envolvidos com responsividade e layout, disponibilizados pelo BootStrap5.
Com isso, os conceitos abordados e estudados foram:
<ol>
  <li>
    Breakpoints
  </li>
  <li>
    Classes conteiner, conteiner-fluid e conteiner-{breakpoint}
  </li>
  <li>
    Layout em Grid
  </li>
  <li>
    Estilização e Formatação das Colunas em Layout Grid
  </li>
</ol>

<br>
Para visualização do conteúdo estudado, as práticas envolvidas estão neste repositório. <br>
Eventualmente no futuro, pretendo terminar o devido curso para ter conhecimento maior e mais amplo do framework. <br>
Por fim, deixarei registrado aqui as anotações que fiz deste curso.

---

<h2> O que é bootstrap? </h2>

- Framework voltado para css
- Focado em responsividade
- Possui recursos para padronizar design entre diferentes tipos de layouts (entre desktop e mobile)
- É uma biblioteca de classes css
- Trabalha com diversos padrões e alternativas para estilizar os componentes e layouts

- Permite criar sites modernos, responsivos e atraentes, tendo em vista que suas classes trabalham com problemas em comum ao desenvolver para web.

<h2> Breakpoints para criação de layouts responsivos </h2> 
• Design Responsivo: criar versões de layouts diferentes para diferentes tipos de dispositivos (saída da imagem) <br> <br>
• Breakpoints: representam algumas possíveis larguras (em px) de telas. Assim, eles serão usados para definir estilos (e layout) para uma determinada tela. <br> <br> 
O sistema de layout do BootStrap5 prioriza os dispositivos móveis primeiro. Assim, o programador precisa adicionar classes de breakpoints aos seus componentes caso o mesmo seja utilizado em dispositivos com telas maiores. <br> <br>

• <b> Tabela com uso de breakpoints </b>
<table>
  <thead>
    <tr>
      <th>Breakpoint</th>
      <th>Class infix</th>
      <th>Dimensions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>X-Small</td>
      <td><em>None</em></td>
      <td>&lt;576px</td>
    </tr>
    <tr>
      <td>Small</td>
      <td><code>sm</code></td>
      <td>≥576px</td>
    </tr>
    <tr>
      <td>Medium</td>
      <td><code>md</code></td>
      <td>≥768px</td>
    </tr>
    <tr>
      <td>Large</td>
      <td><code>lg</code></td>
      <td>≥992px</td>
    </tr>
    <tr>
      <td>Extra large</td>
      <td><code>xl</code></td>
      <td>≥1200px</td>
    </tr>
    <tr>
      <td>Extra extra large</td>
      <td><code>xxl</code></td>
      <td>≥1400px</td>
    </tr>
  </tbody>
</table>
<br>

Dessa forma, esses infixos estarão no meio do nome das classes para definir um breakpoint.
<br> <br>
Quando a largura de uma tela é maior que todas as classes breakpoint do componente, a classe com maior breakpoint será utilizada.	

<h2> Contêineres para criação de layouts responsivos </h2>

O Bootstrap permite utilizar classes de contêineres que possuem larguras fixas ou variáveis. Com isso é possível criar layouts responsivos.

Há três classes de container:
- <b>container:</b> 
	que define uma largura máxima em cada ponto responsivo de breakpoint

- <b>container-fluid:</b>
	100% em todos os breakpoint

- <b>container-{breakpoint}:</b> 
	que é de largura: 100% até breakpoint especificado
<br><br>
- <b> Tabela com uso de conteiners </b>
<table>
  <thead>
    <tr>
      <td class="border-dark"></td>
      <th scope="col">
        Extra small<br>
        <span class="fw-normal">&lt;576px</span>
      </th>
      <th scope="col">
        Small<br>
        <span class="fw-normal">&ge;576px</span>
      </th>
      <th scope="col">
        Medium<br>
        <span class="fw-normal">&ge;768px</span>
      </th>
      <th scope="col">
        Large<br>
        <span class="fw-normal">&ge;992px</span>
      </th>
      <th scope="col">
        X-Large<br>
        <span class="fw-normal">&ge;1200px</span>
      </th>
      <th scope="col">
        XX-Large<br>
        <span class="fw-normal">&ge;1400px</span>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row" class="fw-normal"><code>.container</code></th>
      <td class="text-muted">100%</td>
      <td>540px</td>
      <td>720px</td>
      <td>960px</td>
      <td>1140px</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-sm</code></th>
      <td class="text-muted">100%</td>
      <td>540px</td>
      <td>720px</td>
      <td>960px</td>
      <td>1140px</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-md</code></th>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td>720px</td>
      <td>960px</td>
      <td>1140px</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-lg</code></th>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td>960px</td>
      <td>1140px</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-xl</code></th>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td>1140px</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-xxl</code></th>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td>1320px</td>
    </tr>
    <tr>
      <th scope="row" class="fw-normal"><code>.container-fluid</code></th>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
      <td class="text-muted">100%</td>
    </tr>
  </tbody>
</table>
<br>
Os contêineres também se utilizam de breakpoints para determinar pontos onde que o layout passa a ter um tipo de comportamento.

<h2>Sistema de layout em grid</h2>

- Grids utilizam flex-box internamente
- Um grid divide um contêiner virtualmente em 12 colunas, de mesma largura. Assim, é possível definir layouts responsivos.
- Além, é possível realizar um agrupamento dessas colunas e fazer uma configuração conforme a necessidade.
- Para utilizar um grid, é necessário criar uma div dentro de um container e utilizar as classes "row" e "col"

<br> 
Exemplo de código

```
<div class="container">
        <h1> Grid com colunas pre-definida</h1>
        <div class="row">
            <div class="col-3 bg-info bg-opacity-25 h100"> Coluna 1 </div>
            <div class="col-6 bg-info bg-opacity-50 h100"> Coluna 2 </div>
            <div class="col-3 bg-info bg-opacity-75 h100"> Coluna 3 </div>
        </div>
  </div>
```

Ao utilizar as classe de utilização de grid, o tamanho da coluna pode ser:
- Tamanho pré-definido: <i>class="col-3"</i>, por exemplo. Assim, define uma configuração de que a div terá 3 colunas do grid.
- Tamanho adaptativo: <i>class="col"</i>, por exemplo. Assim, define que a coluna irá se adaptar a linha do grid em questão, assumindo o valor necessário até ter 12 colunas.
- Além disso, é possível utilizar layout com grid responsivo. Para isso basta usar as classes com os infixos de breakpoints <br>


Exemplo de código

```
       <div class="container">
            <h1> Layout comum para websites com responsividade</h1>
            <div class="row">
                <div class="col-12 bg-dark bg-opacity-25 h100"> Cabeçalho </div>
                 <div class="col-12 col-md-3 bg-dark bg-opacity-50 h400"> Menu </div>
                <div class="col-12 col-md-9 bg-dark bg-opacity-75 h400"> Conteúdo </div>
                <div class="col-12 bg-dark bg-opacity-25 h100"> Rodapé </div>
            <div>
        </div>
```

<h2>Formatação de colunas em layout grid</h2>

- <b>Alinhamento vertical:</b> Irá alinhar as divs e seu conteúdo ao contêiner verticalmente, desde que a altura das divs seja menor que a do contêiner.
```
  <div class="row align-items-<star|end|center>">
```

- <b>Alinhamento por colunas(div):</b> A própria coluna alinha seu conteúdo ao contêiner. Podendo ser no início, meio ou fim entre o espaço disponível do container.
```
<div class="col-3 align-self-<start|end|center>">
```

- <b>Breakpoint:</b> a classe <i>row</i> aceita os infixos de breakpoint. Assim, é possível ter responsividade com manipulação de colunas de um grid.
```
<div class="row align-items-lg-center ">
```

- <b>Alinhamento Horizontal </b>: irá alinhar as divs(colunas) ao conteiner horizontalmente.
```
<div class="row justify-content-<end|center|between|around|evenly|start>">
```

- <b> Mudar ordem de exibição das divs: </b> basta utilizar a classe<i> order-<last|first> </i> ou <i>order-<1|2|..|x> </i>'
```
   <div class="container">
        <h2>Alterando ordem das div</h2>
        <div class="row justify-content-evenly">
            <div class="col-3 order-last">DIV 1</div>
            <div class="col-3 order-first">DIV 2</div>
            <div class="col-3 order">DIV 3</div>
        </div>
    </div>
```

- <b>Espaçamento </b>: a classe <i>offset</i> vai adicionar um espaço de coluna a sua esquerda
```
<div class="col-3 offset-1 ">DIV 2</div>
```

- <b> Adicionando margem automática a esquerda:</b> uso da classe <i>ms-auto</i>. Por ser automático, vai dividir o tamanho da margem entre as duas divs ao espaço do container
```
<div class="col-3 ms-auto">DIV 1</div>
<div class="col-3 ms-auto ">DIV 2</div>
```

- <b>Adicionando margem automática</b>: classe <i>mx-auto</i> (margin horizontal - representa o eixo X)
```
 <div class="col-3 mx-auto">DIV 1</div>
```


