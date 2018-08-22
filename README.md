# Plano de Aulas

> Plano de aulas para a semana do dia 13/08/2018 - 17/08/2018, sobre HTML e CSS básico.
> Este repositório será populado conforme o andamento das aulas.

---


## Obrigada às nossas contribuidoras!!
Esse material foi criado colaborativamente pela equipe Reprograma e com a ajuda de voluntárias.
Nos ajudaram com o layout dos exercícios e implementação no Figma:
- [Rafaella Volkmann](http://ralfa.me/)
- [Sandy Zambeli](https://www.behance.net/sandyzambe950b)

Nos ajudaram com a resolução dos exercícios:
- [Luciana Primante](https://github.com/lprimante)
- [Monique Rodrigues](https://github.com/MoniqueRodrigues)
- [Natalia Izui](https://github.com/natizui)
- [Pamella Azevedo](https://github.com/pamellaazevedo)


**Muito obrigada!!**


---

## Issues - como utilizar nesse repositório
As issues neste repositório podem ser usadas como formas de enviar perguntas acerca do assunto da semana de fundamentos de HTML e CSS.
Para fazer a sua pergunta, basta escrever um resumo dela na área do título e uma descrição sobre problema ou dúvida.

Na descrição, é recomendável ser o mais específica possível. Se possível, colocar **partes do seu código** em HTML e CSS ou **link para o seu repositório** para referência. Especificar também o **navegador** utilizado e o tamanho de tela.
Veja o exemplo na aba Issues. Para documentação de formatação de textos do Github, acesse esse [link](https://guides.github.com/features/mastering-markdown/).

---

### Aula 01 - Introdução à HTML e CSS

Iniciaremos com assuntos básicos de estrutura, nomenclatura e anatomia de HTML e CSS.
- [Editores de texto e organização de pastas](#editores-de-texto);
- [HTML: anatomia e introdução de tags](#html);
- [CSS: anatomia e introdução de propriedades](#css);
- [Classes, id](#classes-e-id);
- [Github Desktop](#github-desktop).

#### Editores de texto
Para se modificar um arquivo .html e .css, precisamos de editor de texto. Apesar de que um simples bloco de notas pode ser a ferramenta para criação desses arquivos, vários softwares foram lançados no mercado para gostos dos programado res, oferecendo facilidades e plugins para facilitar o desenvolvimento. Alguns famosos e notáveis são:
- [Sublime Text](https://www.sublimetext.com/);
- [Notepad++](https://notepad-plus-plus.org/);
- [Atom](https://atom.io/);
- O que vamos usar durante as aulas é o [Visual Studio Code](https://code.visualstudio.com/);

A estrutura de pastas básicas é:
> css
>   style.css
> img
>   imagem.jpg
> index.html
Ou seja, uma pasta com um arquivo index.html na raiz e duas pastas: uma css para inserção de nossos estilos .css e outra img, para inserção de nossas imagens.


#### HTML
HTML é uma abreviação de **Hyper Text Markup Language** (linguagem de marcação em hipertexto). Ou seja, não se trata de uma linguagem de programação, pois não tem lógica (algoritmos, processos etc). Ele cria a **estrutura** de uma página ou aplicação web, determinando a separação de layout e seu conteúdo.

Documentos .html possuem tags de estruturação básica:
```html
<!doctype html>
<html>
    <head></head>
    <body></body>
</html>
```

Internamente, as tags html possuem uma anatomia básica também:
```html
<nome-da-tag atributo="valor do atributo">
    conteúdo
</nome-da-tag>
```

Comentários em HTML:
```html
<!-- Isso é um comentário. Comentários em qualquer linguagem são pedaços de código que são ignorados na renderização (na leitura do computador), mas são úteis para entedimento humano -->
```

#### CSS
CSS é abreviação de **Cascading Style Sheet** (folha de estilos em cascata). É a linguagem que define **estilos** para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração *hierarquia de seletores* e de chamadas de estilo (inline, internal e external).

Para fazer o link de um arquivo .css em um documento .html, devemos inserir a tag <link> no <head> do documento, com o href do caminho do arquivo.
```html
<!doctype html>
<html>
    <head>
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body></body>
</html>
```

Dentro do arquivo .css, a anatomia é:
```css
seletor {
    propriedade: valor;
}
```

Exemplo:
```css
p {
    color: red;
}
```

Comentários em CSS:
```css
/* Sou um comentário CSS */
```


> **ATENÇÃO!**
> Não esqueçam de **indentar** o código! Isso ajuda na sua legibilidade, manutenção e colaboração com outros desenvolvedores.
> Para indentar, selecione a linha do código e aperte *tab*.

#### Classes e id
Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da <body>. Eles são **atributos de nomeação**, sendo class muito usada para referência em CSS e id para Javascript (apesar de que há outras boas práticas no mercado atualmente).
Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser **únicos**.


#### Propriedades e tags
Verificar os arquivos de exercícios para vê-los em prática.

HTML | CSS
------------ | -------------
Tags de **estrutura**: !doctype, html, head, body | Propriedades de **background**: background-imagem, background-color
Tags no **head**: meta (charset), title, link | Propriedades de **texto**: text-align, font-family, font-size, text-decoration, font-size, text-transform
Tags de **divisão**: div | Propriedades de **layout**: width, margin, padding, display (inline-block)
Tags de **texto**: h1 ao h6, p | Propriedade de **cor**: color
Tag de **link**: a | Propriedade de **decoração**: box-shadow, border
Tag de **imagem**: img |

**Macete de centralização**: apenas para elementos block.
1. Definir um tamanho para seu elemento através da propriedade width;
2. Definir margin: 0 auto;


#### Github Desktop
Github é uma rede de repositórios de códigos abertos, muito utilizada por desenvolvedores.
Para a primeira semana, vamos utilizar a versão software do [Github](https://desktop.github.com/).

##### Meu primeiro repositório sem afobação

**NO GITHUB.COM**
1. Crie uma conta em https://github.com
2. No seu perfil, crie um repositório. Defina o nome do seu repositório, uma descrição e crie em *Create repository*.

**NO GITHUB DESKTOP**
1. Na interface do *Github Desktop*, efetue o log in na sua conta.
2. Vá em File > Clone Repository (ou ctrl + shift + O).
3. Na lista de repositórios, selecione aquela que você acabou de criar. Veja onde está o endereço do *Local path*. Lá é para onde você vai copiar seus arquivos para subir para o Github.com.
4. Apertando ok, vá para a pasta do *local path*, copie seus documentos que quer subir para ela.
5. Na interface do *Github Desktop*, você deve ver a listagens de arquivos modificados ou adicionados à esquerda.
6. Na esquerda abaixo, escreva uma mensagem no campo *Summary* e clique em Commit to master. Depois isso NÃO SE DESESPERE: seus arquivos vão sumir de vista. **ISTO ESTÁ CORRETÃO**
7. Depois disso, acima, clique em Push ou Publish. Veja a página do seu repositório do github.com para ver seus arquivos lindos na nuvem.

---

### Aula 02 - Listas e Display

Na parte da manhã, teremos contato com a versão desktop do Github, onde vamos subir todos os nossos exercícios a partir desse momento.
Na parte da tarde, veremos display e listas.
- [CSS: cascata em external, internal e inline](#css-external-internal-e-inline);
- [Metodologia BEM](#método-bem).
- [Documentação HTML e CSS](#documentação-html-e-css);
- [Conceito de display inline, block e inline-block](#display-inline-block-e-inline-block);
- [Listas ordenadas e não ordenadas](#listas-ordenadas-e-não-ordenadas);
- [Pseudo-classes: hover, active, focus e visited](#pseudo-classes);

#### CSS: external, internal e inline
A chamada de marcação de estilo pode ser feita de três formas:
- External: fazendo um link por uma tag na head, para conectar a um estilo externo.
```html
<head>
    <link href="https://fonts.googleapis.com/css?family=Lato:400,700" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>
```
- Internal: ainda no head, abrir uma tag style permite a inserção de código de marcação direto no html.
```html
<head>
    <style>
        p {
            color: red;
        }
    </style>
</head>
```
- Inline: estilo de css que é inserido como atributo em uma tag.
```html
<p style="color: red;">
```
Sobre as prioridades, o inline tem a máxima prioridade, enquanto o external tem a menor.
inline > internal > external.
Por esse motivo, por questões de responsividade e de escalabilidade do código, não vamos trabalhar com estilos inline nem internal.
Para trabalharmos questões de hierarquia, vamos tentar ser mais específicas em nossos seletores no CSS externo.


#### Método BEM
O [método BEM](https://en.bem.info/methodology/quick-start/) é um sistema de nomenclatura de aplicações e documentos web, criado pela Yandex. O método, que define um sistema lógico e coerente de nomenclatura de arquivos e códigos de linguagens como HTML, CSS e Javascript, divide as partes em:
*BEM : block | element | modifier*



**block**: propósito. O que é isso? Ele é semanticamente independente de outros elementos. Exemplos são: section, menu, error, button, header, logo, search-form, form.
- O bloco não deve influenciar seu ambiente, ou seja, não deve haver margin, padding ou position nesse objeto;
- Eles podem estar um dentro do outro (nesting);



**element**: uma parte do *block* que não pode ser usado separadamente dele.
Nome: block-name__element-name, search-form__input, search-form__button.
- Elementos podem estar dentro de um outro elemento;
- Elementos são *sempre* parte de um block, não de um outro elemento. Ou seja, não pode haver uma classe do tipo block__elem1__elem2 (sugestão: block__elem1-elem2 ou block__elem2);
São opcionais, nem todos os blocks tem elementos.

> Block ou element?
> Block: se a seção de código tem a chance de ser re-utilizada e não depende de outros elementos da página para ser implementado.
> Element: se a seção de código não pode ser usada separadamente de um parent (block).



**modifier**: define *aparência*, *estado* ou *comportamento* de um block ou element. Seu nome define sua aparência. Qual o seu tamanho? Qual o seu tema? Exemplos: size_s, theme_islands. Ele é separado do nome do block ou element por um _. Exemplos: block-name_modifier-name e block-name__element-name_modifier-name.
Usos:
- Estados: true, false, enabled e disabled. Estados true não precisam de modifier. search-form__button_disabled.
- Valores: tamanhos, design. search-form__button_size_s, search-form_theme_islands.
- Modifiers não podem ser usados sozinhos.



**mix**: técnica de usar diferentes entidades de BEM. Combine o comportamento e estilo de múltiplas entidades sem duplicar o código e crie componentes de UI semanticamente, baseado nos já existentes.
Por exemplo: btn btn_purple. O mix btn  é uma classe independente do btn_purple, e pode ser usada em outros lugares do documento.


#### Documentação HTML e CSS
É importante saber onde consultar quando houver dúvida sobre tags de HTML, seletores e propriedades de CSS. Existem várias fontes de documentação.
- [Tags de HTML - W3Schools](https://www.w3schools.com/tags/default.asp);
- [Propriedades de CSS  - W3Schools](https://www.w3schools.com/cssref/default.asp);
- [Seletores de CSS - W3Schools](https://www.w3schools.com/cssref/css_selectors.asp);
- [Documentação HTML - MDN](https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5);
- [Documentação CSS - MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS);
- [Várias documentações](https://devdocs.io/).

As documentações da MDN estão parcialmente na língua portuguesa. Quem tem conhecimento de inglês pode contribuir traduzindo seus artigos para o português e deixar a documentação mais acessível.


#### Display inline, block e inline-block
Toda tag em HTML tem por padrão algum valor de display. Os três mais básicos são inline, block e inline-block, cujo entendimento é de extrema importância para manipulação eficiente de elementos na sua página web.

**Block**: são elementos que "ocupam" toda a largura do elemento pai, fazendo com que não deixe outros elementos do lado dele. Mesmo que seja forçado a ter uma medida menor (a partir de propriedade width), ele não deixa outro elemento na mesma linha horizontal.
- Podem conter outros tipos de elementos (inline, block e inline-block);
- Pode estar dentro somente de outros elementos block;

**Inline**: são elementos que ocupam somente o espaço do conteúdo.
- Não podem conter elementos block;
- Podem estar dentro de qualquer tipo de elemento (block, inline, inline-block);
- Não cria linhas novas;
- Não se consegue definir propriedades de width e height para ele.


![Imagem explicativa dos vários tipos de display](https://i.stack.imgur.com/mGTYI.png)


**Inline-block**: são elemento híbridos, que permitem que outros elementos fiquem um ao lado do outro (em linha), mas que também possam receber valores de width e height.
> Fonte da imagem: https://stackoverflow.com/questions/9189810/css-display-inline-vs-inline-block

#### Listas ordenadas e não ordenadas
Listas são usadas para enumeração de items. No HTML, eles também são utilizados para marcação de outros elementos, como itens de menu de navegação.
Para criar uma lista *ordenada*, devemos fazer:
```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

Para criar uma lista *não ordenada*, devemos fazer:
```html
<ul>
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
</ul>
```


#### Pseudo-classes
Pseudo-class são palavras que são adicionadas aos seletores, para especificar um estado especial.
Para tags de link (a), são comuns as pseudo-classes de:
- a:hover (é ativada quando o mouse fica sobre o elemento);
- a:active (quando o link é clicado);
- a:focus (quando o link é focado, através de navegação por tab ou por clique. É importante para acessibilidade. Por padrão aparece um contorno azul no elemento focado);
- a:visited (quando o link já foi visitado, de acordo com o histórico do navegador do usuário).


HTML | CSS
------------ | -------------
Tags de **lista**: ul, ol, li | Propriedades de **layout**: box-sizing, display (inline, block, inline-block)
Tag de **layout**: span | Propriedades de **animação**: transition
 | Propriedades de **alinhamento**: vertical-align


---

### Aula 03 - HTML5 e Navegação

- [Playground para front-end: Codepen](https://codepen.io/);
- O que é HTML5? HTML semântico e suas tags;
- [Coding Dojo, Saiba mais - Link](https://www.devmedia.com.br/o-que-e-o-coding-dojo/30517).

#### HTML5 e tags semânticas
HTML5 foi uma grande atualização da linguagem de markup, feita em 2014, que definiu e criou novas maneiras de se mostrar conteúdo multimídia (vídeo, áudio etc) e deixar o documento mais semântico.
O que significa deixar nosso documento mais semântico? Significa deixá-lo mais legível para algoritmos de sites de busca e para outros desenvolvedores.
Ao invés de criar tags div com classes de nav, header, footer, section, foram criadas novas tags com os mesmos nomes.
Exemplo de um documento sem tags semânticas:
```html
<div class="nav">
    <ul class="menu">
        <li>Nav 1</li>
    </ul>
</div>
<div class="header">
    <h1>Título</h1>
</div>
<div class="main">
    <div class="section">
        <p>Lorem</p>
    </div>
</div>
<div class="footer">
    Copyright
</div>
```

Exemplo com tags semânticas:
```html
<nav>
    <ul class="menu">
        <li>Nav 1</li>
    </ul>
</nav>
<header>
    <h1>Título</h1>
</header>
<main>
    <section>
        <p>Lorem</p>
    </section>
</main>
<footer>
    Copyright
</footer>
```
Nota-se que nem todas as classes foram transformadas em tags semânticas, como o menu.

Tags semânticas mais usadas são: header, nav, section, article, main e footer.
![Esquema exemplo de HTML semântico](https://www.w3schools.com/html/img_sem_elements.gif)
[Lista completa de tags semânticas](https://www.w3schools.com/html/html5_semantic_elements.asp)


HTML | CSS
------------ | -------------
Tags **semântico**: nav, header, main, section, article, aside, footer | 

---

### Aula 04 - Tabelas

- Nevegação superior.
- Tabelas: tags e anatomia;

#### Navegação
Para definir barras de navegação, não precisamos saber de mais nenhuma tag nova. Existe, porém uma maneira específica de criá-las. A mais simples barra superior de navegação se faz com uma tag a e ul, uma definindo o logo e outra o menu de navegação.
```html
<nav>
    <a href="#"><img src="img/logo.png"></a>
    <ul class="menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</nav>
```


No CSS, as propriedades são mais usadas para alinhamento dos elementos e posicionamento fixo na parte superior da página.
```css
nav {
    position: fixed;
    top: 0;
    width: 100%;
}

.menu {
    display: inline-block;
}

.menu li {
    display: inline-block;
}
```
Essas são as propriedades básicas para alinhar todos os elementos. Ajustes finos são feitos a partir de padding, margin etc.


#### Tabelas
Tabelas são usadas para organização de certos tipos de informação. Sua estrutura no HTML se faz através de tags como table, thead, tbody, tr, td. Saber o que cada sigla significa em português ajuda muito na hora de entender o uso de cada tag.
- table: tabela;
- thead: table head, ou **cabeça** de tabela;
- tbody: table body, ou **corpo** de tabela;
- tr: table row, ou **linha** de tabela;
- th: table header, ou **cabeçalho** de tabela;
- td: table data, ou **dado** de tabela.
Sendo assim, a estrutura básica de uma tabela é:
```html
<table>
    <thead>
        <tr>
            <th>Cabeçalho 1</th>
            <th>Cabeçalho 2</th>
            <th>Cabeçalho 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dado de coluna 1</td>
            <td>Dado de coluna 2</td>
            <td>Dado de coluna 3</td>
        </tr>
    </tbody>
</table>
```
Existe também o tfoot, que define o footer de uma tabela. Para mais informações, consulte a [documentação](https://www.w3schools.com/html/html_tables.asp).

Podemos também definir quantas colunas ou linhas uma única célula (ou td/th) vai ocupar. Para isso, usamos os atributos *colspan* (para colunas) e *rowspan* (para linhas).

> E CSS em tabelas?
>> Para estilizar nossas tabelas, é comum usar as propriedades de border, padding, text-align. Uma propriedade nova é a [border-collapse](https://www.w3schools.com/cssref/pr_border-collapse.asp), que não deixa as bordas adjacentes "duplicarem". Outra propriedade é o [border-spacing](https://www.w3schools.com/cssref/pr_border-spacing.asp), que define espaçamento entre células (só funciona para border-collapse: separate).

HTML | CSS
------------ | -------------
Tags de **tabela**: table, thead, tbody, th, td, tr | Propriedades de **tabela**: border-collapse, border-spacing
| Propriedades de **transformação**: transform (translate, rotate, scale, skew)



---

### Aula 05 - Formulários

- Formulário: tags e anatomia.

#### Formulários
Formulários são elementos de HTML que são utilizados para capturar dados dos usuários, através de campos de digitação ou seleção. Podemos capturar vários tipos de dados: **texto** (nome, sobrenome, profissão), **números** (idade, quantidade de filhos), **email**, **escolhas** pré-determinadas através de checkbox, radio e dropdown (assunto, formação escolar, interesses), **textos maiores** (comentário, feedback). Para isso, existem várias tags que usaremos no nosso form.

##### Anatomia básica de formulário
```html
<form action="obrigada.html" method="GET">
    <input type="email" placeholder="Seu email">
    <input type="submit" value="Inscrever-se na Newsletter">
</form>
```
Na tag form, o atributo **action** define o que será feito após a submissão bem sucedida do formulário. A URL definida pode ser uma tela de agradecimento ou um script de execução para gravação de dados no backend. Se não há action, após submissão a mesma página será carregada.
Além disso, o atributo **method** define qual o método de envio dos dados para o servidor. O valor pode ser GET ou POST.

Dentro do formulário, podem haver várias tags de captura de dados do usuário. As mais comuns são:
###### input email
```html
<input type="email" name="email" placeholder="Seu email">
```
Captura o email do usuário. Quando se define o type="email", o próprio navegador faz uma verificação simples do input do dado.
Tags de input são tags que **não** possuem fechamento (funcionam como a tag img).
O atributo *placeholder* permite a adição de um texto explicativo sobre qual tipo de dado deve ser inserido no campo.

> O atributo **name** está presente em todos os campos de inserção de dados do usuário e **não** devem ser esquecidos. Ele é uma informação fundamental para o envio de dados para o servidor.


###### input text
```html
<input type="text" name="nome" placeholder="Seu nome">
```
Os inputs de type="text" aceitam todo tipo de textos curtos dentro deles. Portanto, pode-se capturar, por exemplo, nome, sobrenome, profissão etc do usuário.


###### input checkbox
 ```html
 <p>Selecione até 3 plantas</p>
<input type="checkbox" name="planta" value="alecrim"> Eu gosto de Alecrim
<input type="checkbox" name="planta" value="lavanda"> Eu gosto de Lavanda
<input type="checkbox" name="planta" value="zamioculca"> Eu gosto de Zamioculca
```
No input com type="checkbox", o usuário pode selecionar múltiplas opções. O *name* nas tags de input devem ser iguai para sinalizar que são relacionados. O atributo *value* mostra qual o valor será enviado para o backend.


###### input radio
 ```html
 <p>Selecione apenas 1 sabor de pizza</p>
<input type="radio" name="pizza" value="calabresa"> Eu gosto de Calabresa
<input type="radio" name="pizza" value="baiana"> Eu gosto de Baiana
<input type="radio" name="pizza" value="portuguesa"> Eu gosto de Portuguesa
```
No input com type="radio", o usuário pode selecionar apenas 1 opção. O *name* nas tags de input devem ser iguai para sinalizar que são relacionados. O atributo *value* mostra qual o valor será enviado para o backend.


###### select
 ```html
<select name="assunto">
    <option value="contato">Contato</option>
    <option value="sugestao">Sugestão</option>
    <option value="critica">Crítica</option>
</select>
```
O select permite a apresentação de opções de dados a serem escolhidos pelo usuário. Dentro da tag select, deve-se determinar as opções através de tags option.


###### input number
 ```html
<input type="number" name="idade">
```
No input com type="number", o usuário pode apenas digitar números. Com o *hover* do mouse, ele também consegue ver flechas para aumentar ou diminuir o número.


###### textarea
```html
<textarea name="mensagem" cols="30" rows="10"></textarea>
```
Textarea é uma tag que permite a digitação de um texto maior por parte do usuário. Os atributos cols e rows são opcionais e definem o tamanho padrão da caixa de texto.


###### input submit
```html
<input type="submit" value="Enviar Mensagem">
```
Tag necessária para que haja submissão do formulário. Trata-se de um botão que o usuário pode clicar para efetuar o ato de envio de form. O *value*, nesse caso, age como 'placeholder', definindo um texto que vai aparecer dentro do botão.


###### Label e atributos necessários dentro de tags de form
**Label**
É também importante acompanhar as tags de input por outra tag que se chama *label* (etiqueta). Ela serve como auxiliar para informar ao usuário que tipo de dado é esperado dele.
```html
<label for="name">Name</label>
<input type="text" name="name" placeholder="Seu nome">
```
O atributo 'for' (tradução: para) no label deve ter o mesmo valor do name do input correspondente.

**Atributos importantes**
Dentro de toda tag de input, deve haver o atributo *name*. Isso é necessário para fazer a conexão para um possível script para o envio de dados.
O atributo *value* é necessário em tags de opção - *option*, *input type="checkbox*, *input type="radio*. Isso porque o usuário não vai inserir dados diretamente no campo, mas selecionar a opção com valor pré-estabelecido.
O atributo *placeholder*, em tags de input de texto e email, define um texto dentro do campo de dados que pode servir como dica para o usuário.

O atributo *required* é inserido em qualquer tag de *input*, *select* ou *textarea*, em que é obrigatório ser preenchido para que ocorra a submissão do formulário.


HTML |
------------ |
Tags de **formulário**: form, input, select, option, textarea |

