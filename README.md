# Plano de Aulas

> Plano de aulas para a semana do dia 13/08/2018 - 17/08/2018, sobre HTML e CSS básico.
> Este repositório será populado conforme o andamento das aulas.

---

### Aula 01 - Intrudução à HTML e CSS

Iniciaremos com assuntos básicos de estrutura, nomenclatura e anatomia de HTML e CSS.
- [Editores de texto e organização de pastas](#editores-de-texto);
- [HTML: anatomia e introdução de tags](#html);
- [CSS: anatomia e introdução de propriedades](#css);
- [Classes, id](#classes-e-id);
- [Github Desktop](#github-desktop).

#### Editores de texto
Para se modificar um arquivo .html e .css, precisamos de editor de texto. Apesar de que um simples bloco de notas pode ser a ferramenta para criação desses arquivos, vários softwares foram lançados no mercado para gostos dos programadores, oferecendo facilidades e plugins para facilitar o desenvolvimento. Alguns famosos e notáveis são:
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

Vamos falar sobre documentação, o que fazemos quando temos dúvidas, como ler os artigos.



Na parte da tarde, falaremos sobre HTML semântico e navegação.
- O que é HTML5? HTML semântico e suas tags;
- Nevegação superior.

---

### Aula 04 - Tabelas

Neste dia, vamos praticar os conceitos aprendidos até agora e aprenderemos anatomia e usos de tabelas.
- Tabelas: tags e anatomia;
- [Playground para front-end: Codepen](https://codepen.io/).

---

### Aula 05 - Formulários

Falaremos sobre formulários, que tags são usadas para captura de dados do usuário. Além disso, vamos praticar os conceitos estudados até o momento.
- Formulário: tags e anatomia.