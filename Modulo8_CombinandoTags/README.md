# Combinando Tags

### Tag Anchor com Tags de Formatação e Listas

```html
<HTML>
	<HEAD>
	<TITLE>Tag ANCHOR e as tags de formatação</TITLE>
	</HEAD>

<BODY>
	<P><FONT FACE="Calibri" SIZE="5">Combinando a <i>tag</i> ANCHOR com as <i>tags</i> de formatação.</P>
	<OL>
		<LI><A HREF="#Exerc1"><FONT COLOR="green">Reveja o exercício 1</A></FONT><BR>
		<LI><A HREF="#Exerc2"><FONT COLOR="red">Reveja o exercício 2</A></FONT><BR>
		<LI><A HREF="#Exerc3"><FONT COLOR="purple">Reveja o exercício 3</A></FONT><BR>
	</OL>

	<A NAME="Exerc1">
		<H2>Exercício 1</H2>
	</A>
	<A NAME="Exerc2">
		<H2>Exercício 2</H2>
	</A>
	<A NAME="Exerc3">
		<H2>Exercício 3</H2>
	</A>
</BODY>
</HTML>
```

A *tag* ANCHOR é usada para interligar páginas *web*. Por padrão, os navegadores exibem o *link* sublinhado. Caso deseje modificar o formato, você pode combinar a *tag* Anchor com as *tags* de formatação, como a *tag* BOLD e colocar os *links* como itens de uma lista, seja ela ordenada ou não.

### Tag Anchor com Tag Lista e Tag Imagem

```html
<HTML>
	<HEAD>
	<TITLE>Tag ANCHOR e tag IMAGE</TITLE>
	</HEAD>

<BODY>
	<P><FONT FACE="Calibri" SIZE="3">Combinando a <i>tag</i> ANCHOR com a <i>tag</i> IMAGE.</P>
	<UL>
		<LI><A HREF="Produtos.html"><IMG SRC="truck.png">Produtos</A><BR>
		<LI><A HREF="Servicos.html"><IMG SRC="tools.png">Serviços</A><BR>
		<LI><A HREF="Contato.html"><IMG SRC="letter.png">Contato</A><BR>
	</UL>
	</FONT>
</BODY>
</HTML>
```

> Lista + Imagens + Linkg = Thumbnails (imagens de tamanhos reduzidos)

Emborra o HTML permita o uso das tags *HEIGHT* e *WIDTH* para especificar a altura e largura de uma imagem, este recurso não é o mais indicado, já que, mesmo reduzindo as dimensões da imagem na tela, o tamanho do arquivo continua o mesmo.

O procedimento mais adequado é utilizar um programa de imagens (como o Paint, do Windows) para produzir uma versão da imagem com tamanho reduzido.