# Módulo 3 - Criando um Documento HTML

### Exemplo de código HTML

```html
<HTML>

	<HEAD>
	<TITLE>Escola Virtual - Curso de HTML Básico</TITLE>
	</HEAD>

<BODY>
	<P>O objetivo deste curso é fazer com que você seja capaz de criar páginas <I>web</I>, utilizando a linguagem de marcação HTML.</P>
</BODY>

</HTML>
````

> ? Você deve ter observado vários termos em inglês e entre os sinais de < (menor que) e > (maior que), não é mesmo?

Estas palavras são chamadas de ***tags*** e são os elementos básicos de um documento HTML usados para especificar o formato do conteúdo de uma página *web*.

Os sinais < > permitem aos navegadores distinguir as *tags* de um texto comum e o conteúdo delas pode ser digitado tanto em letras maiúsculas, quanto em minúsculas.

### Partes de um Documento HTML

Um documento HTML possui duas partes:

- *Head* (cabeçalho)

- *Body* (corpo)

> No ***head***, você entra com o **título** da página *web*, que será exibido apenas na barra de endereços no navegador.

> No ***body***, você entra com o **conteúdo** da página *web*.

Em ambos podem ser inseridas outras informações.

> ? Observe que cada uma das partes inicia e termina com uma *tag*. Você consegue identificar a diferença entre a *tag* de início e a de fim?

### Tags com Fechamento

Grande parte das *tags* requerem um fechamento e este é idêntico à *tag* de abertura, porém com o sinal **/ (barra)** no início.

- `<HTML>` e `</HTML>`: inicia e encerra um documento HTML.

- `<HEAD>` e `</HEAD>`: inicia e encerra a área de cabeçalho.

- `<TITLE>` e `</TITLE>`: inicia e encerra a linha de título.

- `<BODY>` e `</BODY>`: inicia e encerra a área do corpo (conteúdo) do documento HTML.

- `<P>` e `</P>`: inicia e encerra um novo parágrafo.

> O conteúdo das *tags* pode ser digitado em minúsculo ou maiúsculo.

### Tags sem Fechamento

```html
<HTML>
	<HEAD>
		<TITLE>HTML - TAG BREAK ou BR</TITLE>
	</HEAD>

<BODY>
	Exemplo do uso da tag BREAK <BR> em um texto.<BR>Observe a quebra de linha.
</BODY>

</HTML>
```

Existem algumas *tags* que **não necessitam de fechamento** e sua sintaxe é somente de abertura, como por exemplo, a *tag* ***<Break>*** ou ***<BR>*** que insere uma quebra de linha.

### Salvando um Documento HTML

Como você deve recordar, arquivos gerados pelo **Bloco de Notas** assumem automaticamente a extensão **.txt**. Acontece que este tipo de arquivo **não** pode ser aberto por navegadores.

> ? E então, como visualizar o documento HTML como página *web* para verificar se ele está de acordo com o que você imagina?

Simples, basta salvar o arquivo com extensão **.html**.

### Codificação de Caracteres

Codificação de caracteres é o mecanismo que armazena os símbolos em forma binária no computador, possibilitando a conversão de um símbolo em código e um código em símbolo.

A codificação **UTF-8** é a recomendação atual para codificação na *web* por ser amplamente suportada em navegadores e editores de código, além de ser compatível com praticamente todos os idiomas do mundo. Esta codificação utiliza um número variável de *bytes* para representar símbolos, podendo usar de 1 a 4 *bytes*.

> + Por padrão, os documentos HTML criados no bloco de notas são salvos na codificação ANSI que é considerada obsoleta, uma vez que utiliza um único *byte*, tem limitações na representação de caracteres especiais e possui diferentes versões, ao passo que o UTF-8 usa codificação *multibyte*, representa um grande conjunto de caracteres e possui padronização uniforme nos pontos de código.
