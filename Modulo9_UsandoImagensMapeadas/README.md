# Módulo 9 - Usando Imagens Mapeadas

### O que são Imagens Mapeadas?

Uma imagem mapeada é uma imagem dividida em **diferentes áreas** e cada área é interligada a um documento.

O navegador, primeiramente, identifica a **área da imagem** que você selecionou e então a URL do **documento vinculado** a esta área.

### Tipos de imagens mapeadas

#### ***Server-side*** (no servidor)

Na imagem mapeada ***server-side***, você define um arquivo especial chamado **arquivo de definição das coordenadas** com todos os detalhes da imagem mapeada e armazena este arquivo no servidor.

Quando você seleciona uma **área** da imagem mapeada, o navegador acessa o arquivo de definição das coordenadas no servidor para identificar a **URL** do documento interligado.

#### ***Client-side*** (no cliente)

Na imagem mapeada client-side, você inclui todos os detalhes da imagem mapeada no próprio documento.

### Como Mapear uma Imagem

Primeiramente, deve-se **definir as áreas** da imagem que possuirão *links* para posteriormente, colocar a referida imagem no *site*.

Para realizar este procedimento, usa-se **formas geométricas** como quadrados, retângulos, círculos ou qualquer outro polígono.

Para delinear as formas geométricas na imagem, são utilizadas **coordenadas** **X** e **Y**, que são contadas **pixel a pixel**, tendo como 0 (zero) o ponto esquerdo superior da imagem.

Para cada tipo de **forma**, a inserção de **coordenadas** possui uma **sintaxe** única.

#### Retângulo

**coords="x1, y1, x2, y2"**

(X1 e Y1 são o vértice esquerdo superior e X2 e Y2 são o vértice direito inferior)

#### Círculo

**coords="x, y, r"**

(X, Y são o centro do círculo e R é a medida do raio, em pixels)

#### Polígono

**coords="x1, y1, x2, y2, x3, y3, ..."**

(Todos os vértices do polígono)

### Mapeando uma Imagem

É muito importante lembar que atualmente, quase nenhuma pessoa realiza a operação de descobrimento dos **pontos de coordendas** manualmente. Praticamente, todos os programas **editores de HTML** possuem um **mapeador de imagens** incluso, no qual você desenha as formas geométricas e o programa fornece o **código** pronto.

`<img src="menu.gif" alt="Menu" usemap="#menu">`

**USEMAP**: Atributo demonstrando que será utilizado um mapa na imagem e qual o nome do mapa utilizado.

### A *tag* **MAP**

```html
<HTML>
	<HEAD>
	<TITLE>Escola Virtual - HTML básico</TITLE>
	</HEAD>
<BODY>
	<img src="menu.png" usemap="#menu" border="0">

	<map name="menu">
		
		<area shape="rect" coords="17,17,183,64" href="http://www.fb.org.br" alt="Item 1">

		<area shape="rect" coords="17,77,183,124" href="http://www.ev.org.br" alt="Item 2">

		<area shape="rect" coords="17,137,183,184" href="http://www.educacao.org.br" alt="Item 3">

		<area shape="rect" coords="17,197,185,244" href="http://www.google.com.br" alt="Item 4">

		<area shape="rect" coords="17,257,185,304" href="http://www.fb.org.br" alt="Item 5">

	</map>
</BODY>

</HTML>
```

### A *tag* **AREA**

`<area shape="forma" coords="x, y, x, y, ..." href="URL">`

- `<area`: **Tag AREA** Delimita a **área da imagem** que irá conter o *link*.

- `shape="forma"`: **Atributo SHAPE** Seus valores podem ser ***rect***, para retângulos, ***circle***, para círculos, e ***polygon***, para polígonos.

- `coords="x, y, x, y, ..."`: **Atributo COORDS** Cordenadas **X** e **Y** que delimitam a forma.

- `href="URL">`: **Atributo HREF** **Endereço (URL)** do documento a ser relacionado com determinada área da imagem.