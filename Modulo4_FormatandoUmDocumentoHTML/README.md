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

|     |      |      |       |      |
|:---:|:----:|:----:|:-----:|:----:|
|Aqua |Black |Blue  |Fuchsia|Gold  |
|Gray |Green |Indigo|Lime   |Maroon|
|Navy |Olive |Purple|Red    |Salmon|
|Siena|Silver|Teal  |White  |Yellow|

> As cores em HTML são definidas em notação hexadecimal pela combinação dos valores RGB (*Red*, *Green*, *Blue*).
>
> Os valores em hexadecimal são definidos em três pares de números, começando em 00 (0 em decimal) e terminando em FF (255 em decimal). Cada símbolo hexadecimal começa sempre com o símbolo *hash* (#).
>
> Com a combinação dos três valores é possível obter mais de 16 milhões de cores (255 x 255 x 255).

```html
<HTML>
	<HEAD>
	<TITLE>Atributos encadeados</TITLE>
	</HEAD>

<BODY>
	<P><FONT FACE="Verdana" SIZE="5" COLOR="#3289C7">Frase visualizada com a fonte Verdana, tamanho 5 e em uma das tonalidades da cor azul.</FONT></P>
</BODY>

</HTML>
```

### Inserindo Quebra de Linha

Por padrão, os navegadores encaixa automaticamente o texto da página *web* de acordo com o tamanho de sua janela. Agora, se você desejar quebrar o texto sempre no mesmo lugar, independente da largura da janela do navegador, você pode utilizar a *tag* `<P></P>` (*paragraph*) ou *tag* `<BR>` (*break*).

```html
<HTML>
	<HEAD>
	<TITLE>Quebra de linha</TITLE>
	</HEAD>

<BODY>
	<P>Quando o código HTML não informa ao navegador onde deve ocorrer a quebra de linha.</P>
	<P>O usuário verá o conteúdo de acordo com o tamanho da janela.</P>
</BODY>

</HTML>
```

```html
<HTML>
	<HEAD>
	<TITLE>Quebra de linha</TITLE>
	</HEAD>

<BODY>
	<P>Quando o código HTML não informa ao navegador onde deve ocorrer a quebra de linha.<BR>
	O usuário verá o conteúdo de acordo com o tamanho da janela.</P>
</BODY>

</HTML>
```

> Pode-se observar que a *tag* `<P></P>` insere uma linha entre os parágrafos.
>
> Já a *tag* `<BR>` insere apenas uma quebra de linha.

### Inserindo Linhas Horizontais numa Página *Web*

Para criar uma linha horizontal, você usa a *tag Horizontal Ruling* `<hr>`. Observe o exemplo:

```html
<HTML>
	<HEAD>
	<TITLE>Inserindo linha horizontal</TITLE>	
	</HEAD>

<BODY>
	<HR>
	<B>Dados pessoais:</B><BR>
	Nome:<BR>
	E-mail:<BR>
	<HR>
	<B>Dados bancários:</B><BR>
	Banco:<BR>
	Agência:<BR>
	Conta corrente:<BR>
	<HR>
</BODY>

</HTML>
```

### Criando Subtítulos

Agora, você verá como adicionar títulos e subtítulos em uma página *web*. Para isso, utilizará a *tag Heading* `<Hx></Hx>` onde **x** é um número que representa o nível do tópico. Pode-se criar até 6 subtítulos.

```html
<HTML>
	<HEAD>
	<TITLE>Inserir subtítulos</TITLE>
	</HEAD>

<BODY>
	<HR>
	<H1><B>1. Linguagem de marcação HTML</B></H1>
		<P>O HTML é uma das linguagens de marcação mais utilizada.</P>
	<HR>
	<H2><B>1.1 Breve histórico</B></H2>
		<P>Tudo começou em ...</P>
</BODY>

</HTML>
```

### Adicionando Comentários

Pode-se inserir **comentários** para incluir notas, sugestões e explicações que o internauta não deva ver. Para isso, você usa a *tag* ***Comment***, com a sintaxe \<!--xxxxxx-->

```html
<HTML>
<HEAD>
	<TITLE>Inserir comentários</TITLE>
</HEAD>

<BODY>
	<HR>
	<H1><B>1. Linguagem de marcação HTML</B></H1>

		<!--Esta parte do texto precisa ser revisada. Ficará como comentário.
		<P>O HTML é uma das linguagens de marcação mais utilizada.</P>-->
	
	<H2><B>1.1 Breve histórico</B></H2>
		<P>Tudo começou em ...</P>
</BODY>

</HTML>
```

> Normalmente você usa a *tag* **Comment** para fornecer informações sobre o autor do documento ou para adicionar uma mensagem de *Copyright*.

### *Tag* Preformatted

Por padrão, os navegadores não exibem os espaços extras e linhas em branco de um documento HTML. Observe, na imagem abaixo, que há espaços no início da segunda e quarta linhas para diferenciar os versos da música **Pastorinhas**, de Noel Rosa.

```html
<HTML>
	<HEAD>
	<TITLE>Espaços e linhas em branco</TITLE>
	</HEAD>

<BODY>
	<!--Trecho da música Pastorinha de Noel Rosa (domínio público)-->
	<P>A estrela d'alva no céu desponta
	   E a lua anda tonta com tamanho esplendor
	   E as pastorinhas pra consolo da lua
	   Vão cantando na rua lindos versos de amor.</P>
</BODY>

</HTML>
```

Para que o usuário visualize a página *web* com os espaços e linhas em branco que você definiu no documento HTML, é necessário utilizar a *tag Preformatted* (Pré-formatado), com a sintaxe `<PRE></PRE>`. O navegador exibe o **bloco de texto** exatamente como está descrito no documento HTML.

```html
<HTML>
	<HEAD>
	<TITLE>Espaços e linhas em branco</TITLE>
	</HEAD>

<BODY>
	<!--Trecho da música Pastorinha de Noel Rosa (domínio público)-->
	<PRE>
	<P>A estrela d'alva no céu desponta
	E a lua anda tonta com tamanho esplendor
E as pastorinhas pra consolo da lua
	Vão cantando na rua lindos versos de amor.</P>
	</PRE>
</BODY>

</HTML>
```