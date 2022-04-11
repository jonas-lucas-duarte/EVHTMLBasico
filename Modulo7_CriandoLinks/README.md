# Módulo 7 - Criando Links

### O que são links?

*Links* são conexões pelas quais você conecta páginas que podem ser do mesmo *website*, externas ou ainda conectar páginas a outros documentos.

Os *links* podem ser criados no **texto** e também em outros **elementos** do *website*, como imagens ou itens de um menu.

### Usando a tag Anchor

A *tag* ***ANCHOR*** `<A></A>` (âncora) é utilizada para criar *links* no hipertexto.

`<a href="URL">Texto descritivo</a>`

- `<a`: **A** Abertura da *tag* ANCHOR.

- `href`: **HREF** Atributo usado para especificar a URL do documento linkado ou interligado.

- `"URL"`: **URL** Endereço de página ou documento a ser linkado.

- `</a>`: **/A** Finalização da *tag* ANCHOR.

### Criando Links em Textos

```html
<HTML>
<HEAD>
	<TITLE>Link de um texto</TITLE>	
</HEAD>

<BODY>
	<P><FONT FACE="Calibri" SIZE="4">Inserindo <I>link</I> em um texto.</P>
	<A HREF="http://www.google.com">Clique aqui</A> para acessar o Google.</FONT>
</BODY>

</HTML>
```

Ao especificar uma URL apropriada para um serviço de internet, você também pode linkar ou interligar sua página *web* a esse serviço. Por exemplo, você pode criar um *link* entre sua página e o seu e-mail.

`<a href="mailto:meuemail@meudominio.com">Texto do link</a>`

```html
<HTML>
<HEAD>
	<TITLE> </TITLE>
</HEAD>
<BODY>
	<H1>Links</H1>
	<A HREF="mailto:meuemail@meudominio.com">Entre em contato</A>
</BODY>
</HTML>
```

### Criando links para uma seção na mesma página

A *tag Anchor* também é utilizada para criar *links* de seção.

Você especifica a URL do documento que deseja interligar, com o nome da seção precedido pelo símbolo **#**.

No entanto, será preciso utilizar um atributo que fará o navegador entender para onde deve ir após o usuário clicar no *link* criado. Este atributo é o NAME.

`<A href="#nome da seção">Texto explicativo</A>`

`<A name="#nome da seção">Texto explicativo</A>`

```html
<HTML>
	<HEAD>
		<TITLE>Link para seção</TITLE>
	</HEAD>
<BODY>
	<P><FONT FACE="Calibri" SIZE="3">Inserindo <I>links</I> criando seções.</P>
	<P> Neste exemplo você verá que, quando o texto for muito grande, você poderá criar <I>links</I> que levem o usuário diretamente ao ponto desejado.</P>
	<A href = "#Capítulo I">O que é HTML?</A><BR>
	<A href = "#Capítulo II">Principais comandos</A>
	<BR>
	<BR>
	<A name = "Capítulo I">
	<H2>O que é HTML?</H2>
	<P>HTML é uma das linguagens de marcação mais conhecidas e utiliza um formato simples de código, que pode ser gerado sem a ajuda de aplicativos especiais.</P>
	<P>Para criar um documento HTML, tudo o que você precisa é de um editor de texto ASCII como o NotePad (Bloco de Notas), por exemplo. Se você precisar verificar a formatação do documento durante a criação, pode usar qualquer navegador, pois todos eles são capazes de interpretar o código.</P>
	</A>
	<A name = "Capítulo II">
	<H3>Principais comandos</H3>
	<P>Os comandos são inseridos no código entre os sinais de menor que "<" e maior que ">" e são chamados de <I>tags</I>.</P>
	</A>
	</FONT>
</BODY>
</HTML>
```

### Criando links com imagens

Basta combinar a *tag Anchor* e a *tag Image*.

`<a href="URL"><img src="img_url"></a>`

- `<a href="URL">`: ***Tag*** **ANCHOR** Para criação de *links*.

- `<img src="img_url">`: ***Tag*** **IMG** *Tag* de inserção de imagem na página.

- `</a>`>: ***Tag*** **ANCHOR** Finalização da tag de *link*.