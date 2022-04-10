# Módulo 6 - Inserindo Imagens

### Tipos de Imagens

Os formatas mais utilizados:

- **JPEG** ou **JPG**

*Joint Photographic Expents Group*

É o método **mais utilizado** para comprimir **imagens fotográficas**. Foi introduzido em 1983 e suporta até **16,8 milhões de cores**. Não permite imagens com fundos transparentes.

- **GIF**

*Graphics Interchange Format*

Foi introduzido pela CompuServe em 1987 e desde então foi amplamente utilizado na *web*. Seu formato suporta oito *bits* por *pixel*, permitindo o uso de uma paleta de até **256 cores**. Utiliza o tipo de compressão LZW e é mais indicado para gráficos, ícones e imagens que não necessitam de muitas cores. Permite imagens com **fundo transparente**.

- **PNG**

*Portable Networks Graphics*

É o **substituto do formato GIF**. No início de 1995 o padrão de compreensão LZW foi patenteado pela empresa Unisys, que anunciou cobrança de *royalties* para o uso deste tipo de arquivo. Esta informaçãp, aliada à crescente capacidade de exibição de cores dos computadores, levou à criação do PNG, que assim como JPG, permite exibição de até **16,8 milhões de cores** e, como o GIF, **fundos transparentes**.

### Inserindo Imagens

A *tag* utilizada para se inserir imagens é a `<IMG>`, utilizada com alguns atributos.

Em primeiro lugar, como já é de se imaginar, você precisará informar ao navegador onde a imagem se encontra, ou seja, o endereço e nome dela. Para isso, utilizaremos o atributo SRC que é a abeviação e *source* (fonte).

Sintaxe: `<IMG SRC="C:\pasta\nomeImagem">`

```html
<HTML>
<HEAD>
	<TITLE>Inserindo imagem</TITLE>	
</HEAD>

<BODY>
	<P>Inserindo a logo da Fundação Bradesco na página <I>web</I>.</P>
	<IMG SRC="logo_FB.png">
</BODY>
</HTML>
```

### Alinhando uma Imagem

O atributo a ser utilizado em conjunto com a *tag* para alinhar a imagem é **ALIGN**.

**align=TOP**

Para deixar a imagem no **topo** do texto, a sintaxe é a seguinte:

`<img src="nomeDaImagem" align="top">`

```html
<HTML>

<BODY>
	<p>Exemplo de texto. <img src="estrela.png" align="top"> Exemplo de texto.</p>	
</BODY>

</HTML>
```

**align=BOTTOM**

Para deixar a imagem **abaixo** do texto, a sintaxe é a seguinte:

`<img src="nomeDaImagem" align="bottom">`

```html
<HTML>

<BODY>
	<p>Exemplo de texto. <img src="estrela.png" align="bottom"> Exemplo de texto.</p>	
</BODY>

</HTML>
```

**align=MIDDLE**

Para deixar a imagem no **meio** do texto, a sintaxe é a seguinte:

`<img src="nomeDaImagem" align="middle">`

```html
<HTML>

<BODY>
	<p>Exemplo de texto. <img src="estrela.png" align="middle"> Exemplo de texto.</p>	
</BODY>

</HTML>
```

**align=RIGHT**

Para deixar a imagem à **direita** do texto, a sintaxe é a seguinte:

`<img src="nomeDaImagem" align="right">`

```html
<HTML>

<BODY>
	<p>Exemplo de texto. <img src="estrela.png" align="right"> Exemplo de texto.</p>	
</BODY>

</HTML>
```

**align=LEFT**

Para deixar a imagem à **esquerda** do texto, a sintaxe é a seguinte:

`<img src="nomeDaImagem" align="left">`

```html
<HTML>

<BODY>
	<p>Exemplo de texto. <img src="estrela.png" align="left"> Exemplo de texto.</p>	
</BODY>

</HTML>
```

### Usando o Atributo ALT

Caso o navegador não consiga exibir a imagem, o atributo **ALT** permite vincular um **texto explicativo** a ela.

Este atributo é considerado de acessibilidade, já que é importantíssimo para **deficientes visuais**, uma vez que os programas desenvolvidos para eles leem as imagens.

Quando o usuário coloca o mouse sobre a imagem, o texto alternativo também é exibido.

Sintaxe: `<IMG ALT="Texto explicativo">`