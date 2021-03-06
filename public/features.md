Features
===

Introduction
===
<i class="fa fa-file-text"></i> HackMD is a realtime collaborate markdown note in all platforms.
This mean you can do some notes with any other in **Desktop, Tablet or even Phone**.
You can Sign in via **Facebook, Twitter, GitHub, Dropbox** in the **[homepage](/)**.

This service still in early stage, might be buggy or crash.
Please report issue in [GitHub](https://github.com/hackmdio/hackmd).
If you need instant help, please use [Facebook Message](https://www.facebook.com/messages/866415986748945).
**Thank you very much!**

Workspace
===
## Modes
**Desktop & Tablet**

<i class="fa fa-edit fa-fw"></i> Edit: See only the editor.
<i class="fa fa-eye fa-fw"></i> View: See only the result.
<i class="fa fa-columns fa-fw"></i> Both: See both in split view.

**Mobile**

<i class="fa fa-toggle-on fa-fw"></i> View: See only the result.
<i class="fa fa-toggle-off fa-fw"></i> Edit: See only the editor.

## Upload image
You can simply press the camera button <i class="fa fa-camera"></i>.
Or **drag-n-drop** image in editor, even **paste** image works!
It will automatically upload to **[imgur](http://imgur.com)**, nothing to worry :tada:
![](http://i.imgur.com/9cgQVqD.png)

## Share note
If you want to share a **editable** note, just copy the url.
If you want to share a **read-only** note, simply press share button <i class="fa fa-share-alt"></i> and copy the url.

## Save
Currently, you can save to **dropbox** <i class="fa fa-dropbox"></i> or save as **.md** <i class="fa fa-file-text"></i> to local.

## Import
Like save feature, you can also import **.md** from **dropbox** <i class="fa fa-dropbox"></i>.
Or import from your **clipboard** <i class="fa fa-clipboard"></i>, and that can parse some **html** which might be useful :smiley:

## Permission
There is a little button on the top right of the view.
You can change the permission via theres options.
It might be one of below:

<i class="fa fa-leaf fa-fw"></i> Freely: Anyone can edit this note.
<i class="fa fa-pencil fa-fw"></i> Editable: Signed user can edit this note.
<i class="fa fa-lock fa-fw"></i> Locked: Only owner can edit this note.
<i class="fa fa-hand-stop-o fa-fw"></i> Private: Only owner can view and edit this note.

**Only the owner of the note can change the permission**

## Embed
```xml
<iframe width="100%" height="500" src="http://hackmd.io/features" frameborder="0"></iframe>
```

View
===
## Table of content
You can look at bottom right place of the view area, there is a TOC button <i class="fa fa-bars"></i>.
Press that will show current table of content and will emphasis which your section on.
Support up to **three header levels**.

## Permalink
Every header will automatically add a permalink on the right side.
You can hover and click <i class="fa fa-chain"></i> to anchor on it.

Edit
===
## Shortcut keys
Just like sublime text, which is pretty quick and convinent.
> For more infomations, see [here](https://codemirror.net/demo/sublime.html).

## Auto complete
This editor provide full auto complete hint of markdown.
- Emojis: type `:` to show hint.
- Code blocks: type ` ``` ` and plus a character to show hint. <i hidden>```</i>
- Headers: type `#` to show hint.
- Referrals: type `[]` to show hint.
- Externals: type `{}` to show hint.
- Images: type `!` to show hint.

## Title
This will take the first **level 1 header** as the note title.

## Tags
Using tags like below, these will show in your **history**.
###### tags: `features` `cool` `updated`

## [YAML metadata](https://hackmd.io/IwFgZgxiBsBGCsBaAnPYAORJm07gDMImGAKYnrwDsUI8QA==)
Provide advanced note information to set the browse behavior, visit above link for detail
- robots: set search engine to index or not
- lang: set browse language
- dir: set text direction
- breaks: set to use line breaks

## Emoji
You can type any emoji like this :smile: :smiley: :cry: :wink:
> See full emoji list [here](http://www.emoji-cheat-sheet.com/)

## Todo List
- [ ] Todos
	- [x] Buy some salad
    - [ ] Brush teeth
	- [x] Drink some water

## Code block
We support many code languages, use the auto complete to see the list.
```javascript=
var s = "JavaScript syntax highlighting";
alert(s);
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) + 
             ' class=""';
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      return /\d+[\s/]/g;
  }
}
```
> If you want **line numbers**, type `=` after specify the code block languagues.
> Also, you can specify the start line number.
> Like below, the line number starts from 101:
```javascript=101
var s = "JavaScript syntax highlighting";
alert(s);
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) + 
             ' class=""';
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      return /\d+[\s/]/g;
  }
}
```

> Or you might want to continue the previous code block line number, use `=+`

```javascript=+
var s = "JavaScript syntax highlighting";
alert(s);
```

### Blockquotes tags
> Using like below to specifiy your **name, time and color** to differ the blockquotes.
> [name=ChengHan Wu] [time=Sun, Jun 28, 2015 9:59 PM] [color=#907bf7]
> > Even support the nest blockquotes!
> > [name=ChengHan Wu] [time=Sun, Jun 28, 2015 10:00 PM] [color=red]

## Externals

### Youtube
{%youtube 1G4isv_Fylg %}

### Vimeo
{%vimeo 124148255 %}

### Gist
{%gist schacon/4277%}

### SlideShare
{%slideshare briansolis/26-disruptive-technology-trends-2016-2018-56796196 %}

### Speakerdeck
{%speakerdeck sugarenia/xxlcss-how-to-scale-css-and-keep-your-sanity %}

## MathJax

You can render *LaTeX* mathematical expressions using **MathJax**, as on [math.stackexchange.com](http://math.stackexchange.com/):

The *Gamma function* satisfying $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ is via the Euler integral

$$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}.
$$

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

> More information about **LaTeX** mathematical expressions [here](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).

## UML diagrams

### Sequence diagrams

You can render sequence diagrams like this:

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
Note left of Alice: Alice responds
Alice->Bob: Where have you been?
```

### Flow charts

And flow charts like this:
```flow
st=>start: Start
e=>end: End
op=>operation: My Operation
op2=>operation: lalala
cond=>condition: Yes or No?

st->op->op2->cond
cond(yes)->e
cond(no)->op2
```

### Graphviz
```graphviz
digraph hierarchy {

                nodesep=1.0 // increases the separation between nodes
                
                node [color=Red,fontname=Courier,shape=box] //All nodes will this shape and colour
                edge [color=Blue, style=dashed] //All the lines look like this

                Headteacher->{Deputy1 Deputy2 BusinessManager}
                Deputy1->{Teacher1 Teacher2}
                BusinessManager->ITManager
                {rank=same;ITManager Teacher1 Teacher2}  // Put them on the same level
}
```

> More information about **Sequence diagrams** syntax [here](http://bramp.github.io/js-sequence-diagrams/).
> More information about **Flow charts** syntax [here](http://adrai.github.io/flowchart.js/).
> More information about **Graphviz** syntax [here](http://www.tonyballantyne.com/graphs.html)

## Typography

### Headers

```
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
```

### Horizontal rules

___

---

***


### Typographic replacements

Enable typographer option to see result.

(c) (C) (r) (R) (tm) (TM) (p) (P) +-

test.. test... test..... test?..... test!....

!!!!!! ???? ,,

Remarkable -- awesome

"Smartypants, double quotes"

'Smartypants, single quotes'

### Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Deleted text~~

lu~lala~

Superscript: 19^th^

Subscript: H~2~O

++Inserted text++

==Marked text==


### Blockquotes


> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows. 


### Lists

#### Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

#### Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa


1. You can use sequential numbers...
1. ...or keep all the numbers as `1.`
1. feafw
2. 332
3. 242
4. 2552
1. e2

Start numbering with offset:

57. foo
1. bar

### Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting

``` js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

### Tables

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Right aligned columns

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Left aligned columns

| Option | Description |
|:------ |:----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Center aligned columns

| Option | Description |
|:------:|:-----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |


### Links
[link text](http://dev.nodeca.com)
[link with title](http://nodeca.github.io/pica/demo/ "title text!")
Autoconverted link https://github.com/nodeca/pica


### Images
![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")
Like links, Images also have a footnote style syntax
![Alt text][id]
With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"


### Footnotes

Footnote 1 link[^first].
Footnote 2 link[^second].
Inline footnote^[Text of inline footnote] definition.
Duplicated footnote reference[^second].

[^first]: Footnote **can have markup**
    and multiple paragraphs.
[^second]: Footnote text.

### Definition lists

Term 1

:   Definition 1

with lazy continuation.

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.

_Compact style:_

Term 1
  ~ Definition 1

Term 2
  ~ Definition 2a
  ~ Definition 2b

### Abbreviations

This is HTML abbreviation example.
It converts "HTML", but keep intact partial entries like "xxxHTMLyyy" and so on.

*[HTML]: Hyper Text Markup Language