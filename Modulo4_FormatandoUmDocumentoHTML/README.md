# Módulo 4 - Formatando um Documento HTML

### Inserindo Efeitos

#### Negrito

O efeito negrito (bold) é o mais utilizado para destacar partes de um texto.

- Sintaxe: `<B>Texto</B>`

- Exemplo:

```html
<P>Texto da página <B>web</B>.</P>
```

#### Itálico

O efeito itálico (italic) é utilizado para destacar termos em outro idioma ou citações.

- Sintaxe: `<I>Texto</I>`

- Exemplo:

```html
<P>Texto da página <I>web</I>.</P>
```

#### Sublinhado

O efeito sublinhado (underline) é pouco utlizado para que os usuários não confundam o texto destacado com *links*.

- Sintaxe: `<U>Texto</U>`

- Exemplo:

```html
<P>Texto da página <U>web</U>.</P>
```

### Alterando Alinhamento do Texto

#### P align=LEFT

Texto alinhado à **esquerda** (padrão), a sintaxe é a seguinte:

`<p align=left>Texto.</p>`

```html
<HTML>
	
<BODY>
	<P ALIGN=left>O objetivo deste curso é criar páginas web, utilizando a linguagem de marcação HTML.</P>
</BODY>

</HTML>
```

#### P align=CENTER

Texto **centralizado**, a sintaxe é a seguinte:

`<p align=center>Texto.</p>`

```html
<HTML>
	
<BODY>
	<P ALIGN=center>O objetivo deste curso é criar páginas web, utilizando a linguagem de marcação HTML.</P>
</BODY>

</HTML>
```

#### P align=RIGHT

Texto alinhada à **direita**, a sintaxe é a seguinte:

`<p align=right>Texto.</p>`

```html
<HTML>
	
<BODY>
	<P ALIGN=right>O objetivo deste curso é criar páginas web, utilizando a linguagem de marcação HTML.</P>
</BODY>

</HTML>
```

#### P align=JUSTIFY

Texto **justificado** em ambas as margens, a sintaxe é a seguinte:

`<p align=justify>Texto.</p>`

```html
<HTML>
	
<BODY>
	<P ALIGN=justify>O objetivo deste curso é criar páginas web, utilizando a linguagem de marcação HTML.</P>
</BODY>

</HTML>
```

### Alterando a Fonte

Você deve ter observado, que independente da fonte na qual o código HTML é digitado, a visualização da página *web* é sempre com a mesma fonte, *Times New Roman*. Pois é, essa é a fonte padrão.

Caso você deseje utilizar outra fonte, alterar o tamanho ou ainda a cor, será preciso fazer uso da *tag* `<FONT></FONT>`.

> Você pode, teoricamente, escolher qualquer fonte existente, mas na verdade ela só aparecerá em computadores que tiverem tal fonte instalada.
> 
> Portanto, para isso não acontecer, escolha uma fonte que já venha instalada com o sistema operacional, presente na maioria dos computadores, tais como:
>
> - Arial
>
> - Calibri
>
> - Comic Sans MS
>
> - Verdana

Um dos primeiros atributos utilizados com a *tag* `<FONT>`, é o FACE, que permite alterar o tipo da fonte. A sintaxe fica assim: `<FONT FACE="nome da fonte">`.

```html
<HTML>
	<HEAD>
	<TITLE>Alterando a fonte</TITLE>		
	</HEAD>

<BODY>
	<P>Esta frase será visualizada com a fonte padrão.</P>
	<P><FONT FACE="Comic Sans MS">Esta frase será visualizada com a fonte Comic Sans MS.</FONT></P>
</BODY>

</HTML>
```

Agora que você já sabe alterar o tipo da fonte, veja como alterar o tamanho dela.

Para isso, basta acrescentar o atributo *SIZE* (tamanho) na *tag* `<FONT>`.

A sintaxe fica assim: `<FONT SIZE="numero">`, onde "numero" pode variar de 1 até 7.

```html
<HTML>
	<HEAD>
	<TITLE>Alterando a fonte</TITLE>
	</HEAD>

<BODY>
	<FONT SIZE="1">Tamanho: 1</FONT><BR>
	<FONT SIZE="2">Tamanho: 2</FONT><BR>
	<FONT SIZE="3">Tamanho: 3</FONT><BR>
	<FONT SIZE="4">Tamanho: 4</FONT><BR>
	<FONT SIZE="5">Tamanho: 5</FONT><BR>
	<FONT SIZE="6">Tamanho: 6</FONT><BR>
	<FONT SIZE="7">Tamanho: 7</FONT><BR>
</BODY>

</HTML>
```

### Alterando a Cor da Fonte

A sintaxe fica assim: `<FONT COLOR="cor">` onde "cor" pode ser definida pelo nome ou pelo código hexadecimal da cor.

Ao utilizar o nome, você estará restrito às cores básicas, algumas delas são:

|Aqua|Black|Blue|Fuchsia|Gold|
|:--:|:---:|:--:|:-----:|:--:|
