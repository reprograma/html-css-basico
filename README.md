# Plano de Aulas

> Plano de aulas para a semana do dia 13/08/2018 - 17/08/2018, sobre HTML e CSS básico.
> Este repositório será populado conforme o andamento das aulas.

---

### Aula 01 - Intrudução à HTML e CSS

Iniciaremos com assuntos básicos de estrutura, nomenclatura e anatomia de HTML e CSS.
- Editores de texto e organização de pastas;
- HTML: anatomia e introdução de tags;
- CSS: anatomia e introdução de propriedades;
- Classes, id, links;
- [Github Desktop](https://desktop.github.com/).

##### Editores de texto
Para se modificar um arquivo .html e .css, precisamos de editor de texto. Apesar de que um simples bloco de notas pode ser a ferramenta para criação desses arquivos, vários softwares foram lançados no mercado para gostos dos programadores, oferecendo facilidades e plugins para facilitar o desenvolvimento. Alguns famosos e notáveis são:
- [Sublime Text](https://www.sublimetext.com/);
- [Notepad++](https://notepad-plus-plus.org/);
- [Atom](https://atom.io/);
O que vamos usar durante as aulas é o [Visual Studio Code](https://code.visualstudio.com/);


##### HTML
HTML é uma abreviação de Hyper Text Markup Language (linguagem de marcação em hipertexto). Ou seja, não se trata de uma linguagem de programação, pois não tem lógica (algoritmos, processos etc). Ele cria a estrutura de uma página ou aplicação web, determinando a separação de layout e seu conteúdo.

Documentos .html possuem tags de estruturação básica:
```html
<!doctype html>
<html>
    <head></head>
    <body></body>
</html>
```

No microcosmos, as tags html possuem uma anatomia básica também:
<nome-da-tag atributo="valor do atributo">
    conteúdo
</nome-da-tag>

Comentários em HTML:
<!-- Isso é um comentário. Comentários em qualquer linguagem são pedaços de código que são ignorados na renderização (na leitura do computador), mas são úteis para entedimento humano -->

##### CSS
CSS é abreviação de Cascading Style Sheet (folha de estilos em cascata). É a linguagem que define estilos para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração hierarquia de seletores e de chamadas de estilo (inline, internal e external).

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
seletor {
    propriedade: valor;
}
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
> Não esqueçam de indentar o código! Isso ajuda na sua legibilidade, manutenção e colaboração com outros desenvolvedores.
> Para indentar, selecione a linha do código e aperte *tab*.

##### Classes e id
Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da <body>. Eles são atributos de nomeação, sendo class muito usada para referência em CSS e id para Javascript (apesar de que há outras boas práticas no mercado atualmente).
Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser **únicos**.


##### Propriedades e tags
Verificar os arquivos de exercícios para vê-los em prática.

HTML | CSS
------------ | -------------
Tags de estrutura: !doctype, html, head, body | Propriedades de background: background-imagem, background-color
Tags no <head>: meta (charset), title, link | Propriedades de texto: text-align, font-family, font-size, text-decoration, font-size, text-transform
Tags de divisão: div | Propriedades de layout: width, margin, padding, display (inline-block)
Tags de texto: h1 ao h6, p | Propriedade de cor: color
Tag de link: a | Propriedade de decoração: box-shadow, border
Tag de imagem: img |

Macete de centralização: apenas para elementos block.
1. Definir um tamanho para seu elemento através da propriedade width;
2. Definir margin: 0 auto;


##### Github Desktop
Github é uma rede de repositórios de códigos abertos, muito utilizada por desenvolvedores.
Para a primeira semana, vamos utilizar a versão software do [Github](https://desktop.github.com/).
> Meu primeiro repositório sem afobação
> NO GITHUB.COM
>> Crie uma conta em https://github.com
>> No seu perfil, crie um repositório. Defina o nome do seu repositório, uma descrição e crie em *Create repository*.
> NO GITHUB DESKTOP
>> Na interface do *Github Desktop*, efetue o log in na sua conta.
>> Vá em File > Clone Repository (ou ctrl + shift + O).
>> Na lista de repositórios, selecione aquela que você acabou de criar. Veja onde está o endereço do *Local path*. Lá é para onde você vai copiar seus arquivos para subir para o Github.com.
>> Apertando ok, vá para a pasta do *local path*, copie seus documentos que quer subir para ela.
>> Na interface do *Github Desktop*, você deve ver a listagens de arquivos modificados ou adicionados à esquerda.
>> Na esquerda abaixo, escreva uma mensagem no campo *Summary* e clique em Commit to master. Depois isso NÃO SE DESESPERE: seus arquivos vão sumir de vista. **ISTO ESTÁ CORRETÃO**
>> Depois disso, acima, clique em Push ou Publish. Veja a página do seu repositório para ver seus arquivos lindos na nuvem.

---

### Aula 02 - Listas e Display

Na parte da manhã, teremos contato com a versão desktop do Github, onde vamos subir todos os nossos exercícios a partir desse momento.
Na parte da tarde, veremos display e listas.
- Conceito de display inline, block e inline-block;
- [Metodologia BEM](https://en.bem.info/methodology/html/).
- Listas ordenadas e não ordenadas.

---

### Aula 03 - HTML5 e Navegação

Vamos falar sobre documentação, o que fazemos quando temos dúvidas, como ler os artigos.
- [Tags de HTML](https://www.w3schools.com/tags/default.asp);
- [Propriedades de CSS](https://www.w3schools.com/cssref/default.asp);
- [Várias documentações](https://devdocs.io/).

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