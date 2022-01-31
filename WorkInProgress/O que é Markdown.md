# O que é Markdown?



Markdown é uma linguagem de marcação, assim como o HTML. Ele é um jeito de escrever em texto puro, deixando anotações sobre a formatação.

O Markdown é um sistema de formatação aberto que torna a escrita e a leitura mais simples. Com uma codificação mínima, além de fácil, ele é visualmente mais “limpo”.

# História

Em2004, John Gruber criou a linguagem Markdown em colaboração com Aaron Swartz na sintaxe, buscando possibilitar a escrita em XHTML (ou HTML) estruturalmente válido partindo de textos simples.

Seu principal objetivo quanto ao design é a legibilidade, característica que normalmente é afetada em linguagens de marcação, tais como Rich Text Format (RTF) ou HTML, pela presença de tags ou instruções de formatação “explícitas”. Em Markdown as formatações são muito mais sutis, essa inspira-se nas convenções existentes para marcar um texto simples ou e-mail, apesar de ser baseada em linguagens de marcação anteriores, como setext, Textile e reStructuredText.

Gruber escreveu um script PerlMarkdown.pl , que converte a entrada de texto marcada em XHTML ou HTML válido e bem formado e substitui os colchetes angulares ‘ <’ ‘ >’ e o e comercial ‘ &’ por suas referências de entidade de caractere correspondentes . Ele pode assumir o papel de um script independente, um plugin para Blosxom ou um Movable Type , ou de um filtro de texto para BBEdit .

Markdown foi implementado por outros, por exemplo, em um módulo Perl disponível no CPAN ( Text::Markdown) e em uma variedade de outras linguagens de programação. Ele é distribuído sob uma licença estilo BSD e está incluído ou disponível como um plugin para vários sistemas de gerenciamento de conteúdo .

Variações da linguagem Markdown são amplamente utilizada por sites como GitHub, Bitbucket, Reddit, Diaspora, Stack Exchange, OpenStreetMap e SourceForge para facilitar a comunicação e discussão entre usuários; também é muito utilizada em arquivos do tipo README.

# Criando um arquivo

Para criar um arquivo em markdown, simplesmente salve com a extensão .md

# Ferramentas

Para auxiliar a criação de arquivos markdown existem algumas, como:

- [StackEdit](https://stackedit.io/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Typora](https://typora.io/)
- [Dillinger](https://dillinger.io/)
- Etc…

# Usando o markdown

Omarkdown é convertido em HTML, então se já tiver conhecimento de HTML é mais simples de absorver o conteúdo.

## Comentários

para criar comentários podemos usar a mesma sintaxe do html.

```
<!-- comentário -->
```

## Title

```
# H1## H2### H3#### H4##### H5###### H6<!-- Alternativa para H1 and H2 -->Alt-H1======Alt-H2------
```

## Lista

**Lista desordenada**

Para criar uma lista não ordenada com o markdown podemos usar tanto *, quanto — ou +, todos têm a mesma funcionalidade, para criar uma sublista, apenas insira dois espaço ou um tab no item, exemplo:

```
* Red* Green  * Green  * Blue    * Green    * Blue
```

**Lista ordenada**

Para uma lista ordenada adicione os números:

```
1.  Red2.  Blue3.  Green
```

**Lista de checkbox**

Para uma lista de check adicione os colchetes com espaço, para marcar adicione um X, exemplo:

```
- [ ] Red- [x] Blue- [x] Green
```

## Link

Para criar link [texto a ser exibido](link, “título”).

```
[Google](https://www.google.com,  "Site do Google")
```

Também é possível criar referências de link, exemplo:

```
[referência de texto][Arbitrary case-insensitive reference text][usando referência numérica][1]<!-- Referencias -->[arbitrary case-insensitive reference text]: https://link[1]: http://link "título"
```

Para usar email use, assim cria o mailto: automaticamente, mas também é possível usar a abreviação normal [texto a ser exibido](link, “título”).

```
<email@email.com>
```

## Imagens

Para adicionar imagens ou gif, use:

```
![myImage](https://media.giphy.com/media/lPoxtQlcX30doRbHTN/giphy.gif)
```

Também podemos adicionar referência nas imagens, exemplo:

```
Reference-style:![alt text][logo]<!-- Referencias -->[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"
```

Se quiser personalizar a altura ou largura da imagem use o html diretamente.

```
<img src="https://media.giphy.com/media/lPoxtQlcX30doRbHTN/giphy.gif" width="42" height="42">
```

## Citação

para adicionar citações adicione o sinal de maior que(>), exemplo:

```
> Texto usando citação
```

## Usando códigos

Usando uma crase `, o texto ficará marcado, exemplo:

```
`code`
```

Para usar códigos grande use 3 crases ```, Isto fará com que ele seja envolvido entre uma tag <pre> e vai preservar os espaços e quebras de linha, alguns conversores ao adicionar o tipo de linguagem o código fica mais legível, exemplo:

```
```javapublic static void main(String[] args) {//TODO}```
```

## Estilo de Texto

O markdown possui diversas formas de ajustar o texto.

**Texto em negrito**

Para usar texto negrito use dois asteriscos (**).

```
**texto negrito**
```

**Texto itálico**

Para usar texto itálico use um underscore (_) ou só um asterisco(*).

```
_texto itálico_*texto itálico*
```

**Texto riscado**

Para usar texto riscado use dois til(~~).

```
~~texto riscado~~
```

**Texto sobrescrito**

Para usar texto sobrescrito é necessário usar a tag <sup>.

```
Texto <sup>sobrescrito</sup>
```

**Texto subscrito**

Para usar texto subscrito é necessário usar a tag <sub>.

```
Texto <sub>subscrito</sub>
```

**Texto de entrada de teclado**

Para usar o texto com estilo de teclado use a tag <kdb>

```
<kbd>ALT + F4</kbd>
```

**Texto Marcado**

Para marcar um texto podemos usar a tag <mark>

```
Texto <mark>marcado</mark>
```

## Linha Horizontal

Para criar uma linha horizontal use 3 asteriscos ou sinal de hífen ou underscore.

```
---***___
```

## Centralizando itens

Para centralizar itens no markdown é necessário usar a tag <center>.

```
<center>Item centralizado</center>
```

## Tabela

Escolha os títulos das colunas e use | para delimitar as colunas. Depois, utilize hífen — na segunda linha para indicar que acima estão os títulos das colunas, usando novamente o | para delimitar colunas.

Para especificar o tipo de alinhamento que deseja ter nas tabelas, utilize : ao lado do campo horizontal de hífens — -, na segunda linha da sua tabela. Veja abaixo:

- **Alinhado a esquerda**: usar : no lado esquerdo (alinhamento padrão);
- **Alinhado a direita**: usar : no lado direito;
- **Centralizado**: usar : dos dois lados.

```
| Alinhado a esquerda | Centralizado | Alinhado a direita || :------------------ | :----------: | -----------------: || Valor               | Valor        | Valor              || Valor               | Valor        | Valor              || Valor               | Valor        | Valor              |
```

# Extras

Esses itens abaixo, só funcionam em alguns lugares/ferramentas.

## Barra de progresso

O próprio HTML tem uma tag para progresso e como o markdown converti para HTML, então podemos usar a tag <progress> para criar uma barra de progresso.

```
Barra de progresso <progress value=”32" max=”100"></progress>
```

## Tag Details

A tag <details> é uma tag do html que possibilita criar uma informação e ocultar até ser clicada, exemplo:

```
<details><summary>Clique aqui para exibir</summary>texto oculto</details>
```

## Usando formulas matematica

para usar formulas matematica use o dólar ($), exemplo.

```
$-b \pm \sqrt{b² — 4ac} \over 2a$
```

## Emoji

Para usar emojis, basta usar os códigos:

```
:bowtie:
```

Para mais códigos acesse o [Emoji cheat sheet](https://www.webfx.com/tools/emoji-cheat-sheet/)

[Emoji cheat sheet for GitHub, Basecamp and other servicesHowever some of the emoji codes are not super easy to remember, so here is a little cheat sheet. ✈ Got a modern browser…www.webfx.com](https://www.webfx.com/tools/emoji-cheat-sheet/)

## Obrigado por ler!

Se você tiver alguma dúvida, reclamação ou dica, pode deixar aqui nos comentários. Vou ter o maior prazer em responder!

😊😊 Até mais! 😊😊

[Walter Nascimento | PT-BR](https://medium.com/walternascimentobarroso-pt?source=post_sidebar--------------------------post_sidebar--------------)

**Related**

[![img](https://miro.medium.com/focal/52/52/50/50/0*xu2D-T2guQ1YGeFe.png)21 docker commands with examples | Quick Cheat Sheet](https://medium.com/@chetan.gadgilwar/21-docker-commands-examples-for-daily-work-cheat-sheet-fa554e6f6d19?source=read_next_recirc---------0---------------------38de155c_fbcd_422c_8842_c508a353e75e----------)

[![Overview of the Azure DevOps pipeline deploying a DACPAC with Always Encrypted objects](https://miro.medium.com/focal/52/52/50/50/1*3T8v-bz6_Ifp44fLZGd2zw.png)How to use Azure SQL Always Encrypted in your CI/CD pipeline](https://medium.com/@remy.ursem/how-to-use-azure-sql-always-encrypted-in-your-ci-cd-pipeline-cb35b0c64458?source=read_next_recirc---------1---------------------38de155c_fbcd_422c_8842_c508a353e75e----------)

[![img](https://miro.medium.com/focal/52/52/50/50/0*HsBoR9P5HHVeEPuW.jpg)NS0–527 Exam Questions — NetApp Certified Implementation Engineer — Data Protection](https://karon-bill.medium.com/ns0-527-exam-questions-netapp-certified-implementation-engineer-data-protection-60ba3baf352c?source=read_next_recirc---------2---------------------38de155c_fbcd_422c_8842_c508a353e75e----------)

[![img](https://miro.medium.com/focal/52/52/50/50/0*9V2W46If2KC39sW6)Implementation of Snowpipe in SnowflakeContinuous Data Loading with Snowpipe:](https://medium.com/@shruthimurali31/implementation-of-snowpipe-in-snowflake-e22c7d70377?source=read_next_recirc---------3---------------------38de155c_fbcd_422c_8842_c508a353e75e----------)

- [Markdown](https://medium.com/walternascimentobarroso-pt/tagged/markdown)
- [Markdown Curso](https://medium.com/walternascimentobarroso-pt/tagged/curso-markdown)
- [Treinamento Markdown](https://medium.com/walternascimentobarroso-pt/tagged/treinamento-markdown)
- [Tecnologia](https://medium.com/walternascimentobarroso-pt/tagged/tecnologia)