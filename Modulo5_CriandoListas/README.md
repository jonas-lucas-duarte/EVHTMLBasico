# Módulo 5 - Criando Listas

### Tipos e Funções de Listas

Lista é uma coleção de **itens relacionados**. Você lista para **organizar dados** com uma sequência de passos ou para listar em um grupo.

O HTML possui **dois tipos** de lista:

- Numeradas (ou Ordenada)

	1. São Paulo

	2. Rio de Janeiro

	3. Belo Horizonte

	4. Vitória

- Não Numeradas (ou Não Ordenada)

	- São Paulo

	- Rio de Janeiro

	- Belo Horizonte

	- Vitória

### Criando Listas Ordenadas

```html
<HTML>
<HEAD>
	<TITLE>Criando lista ordenada</TITLE>
</HEAD>	

<BODY>
	<P><FONT FACE="Calibri" SIZE="4">Para criar um documento HTML é necessário seguir os passos abaixo.</P>
	<OL>
		<LI>Acessar o Bloco de Notas.</LI>
		<LI>Indicar através da <I>tag</I> &LT;HTML&GT; o tipo de documento criado.</LI>
	</OL>
	<P>Esses são os primeiros passos para se criar uma página <I>web</I>.</P>
</BODY>

</HTML>
```

Para criar uma lista ordenada, utilizamos duas *tags*:

- `<OL></OL>`: que abre e fecha o tipo de lista

- `<LI></LI>`: abre cada item da lista

### Criando Listas Não Numeradas

```html
<HTML>
<HEAD>
	<TITLE>Criando lista não ordenada</TITLE>
</HEAD>	

<BODY>
	<P><FONT FACE="Calibri" SIZE="4">Segue abaixo lista de materiais necessários:</P>
	<UL>
		<LI>Leads</LI>
		<LI>Conectores</LI>
		<LI>Chave Philips</LI>
		<LI>Alicate</LI>
	</UL>
	<P>Somente comece a instalação, se possuir todos os materiais.</P>
</BODY>

</HTML>
```

Para criar uma lista ordenada, utilizamos duas *tags*:

- `<UL></UL>`: que abre e fecha o tipo de lista

- `<LI></LI>`: abre cada item da lista

### Lista Intercalada

Também é possível criar combinações de listas em uma página *web*. Essa combinação é chamada de **lista intercalada**.

```html
<HTML>
	<HEAD>
	<TITLE>Criando lista intercalada</TITLE>
	</HEAD>
	
<BODY>
	<P><FONT FACE="Calibri" SIZE="4">Principais características dos <i>notebooks</i> pesquisados:</P>
		
	<OL>
	<LI>Orange</LI>
		<UL>
			<LI>Tela sensível ao toque de 13"</LI>
			<LI>3 entradas USB</LI>
		</UL>		
	<LI>Lemon</LI>
		<UL>
			<LI>Tela sensível ao toque de 15"</LI>
			<LI>2 entradas USB</LI>
		</UL>
	</OL>
	<P>Após a análise o grupo deverá escolher a melhor opção para o trabalho a ser realizado.</P>
</BODY>
</HTML>
```

### Personalizando Listas

O atributo **TYPE** pode especificar o tipo de **marcador** em uma lista não ordenada, ou tipo de **números** em uma lista ordenada. Observe, abaixo, os valores que podem ser utilizados.

A : Para exibir letras maiúsculas.

a : Para exibir letras minúsculas.

I : Para exibir números romanos grandes.

i : Para exibir números romanos pequenos.

- Sintaxe: `<OL TYPE="estilo_do_numero">`

DISC : Para exibir (círculo preenchido).

CIRCLE : Para exibir (círculo não preenchido).

SQUARE : Para exibir (quadrado preenchido).

- Sintaxe: `<UL TYPE="estilo_do_numero">`