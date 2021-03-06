# Markdown Examples

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Headings

Headings from `h1` through `h6` are constructed with a `#` for each level:

```markdown
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
```

Renders to:
<div class="md-rendered-html" style="width:300px; padding: 0px 0px 10px 44px;">
  <h1> h1 Heading </h1>
  <h2> h2 Heading </h2>
  <h3> h3 Heading </h3>
  <h4> h4 Heading </h4>
  <h5> h5 Heading </h5>
  <h6> h6 Heading </h6> 
</div>

HTML:
```
<h1>h1 Heading</h1>
<h2>h2 Heading</h2>
<h3>h3 Heading</h3>
<h4>h4 Heading</h4>
<h5>h5 Heading</h5>
<h6>h6 Heading</h6>
```

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Text

Body text is written as normal, wrapped with `<p></p>` tags in the rendered HTML.

So this body copy:

```markdown
Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.
```
Renders to:
<div class="md-rendered-html">
Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.
</div>

and this HTML:

```html
<p>Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.</p>
```
<!-- ------------------------------------------------------------------------------------------------------------ -->

## Lists

### Unordered
A list of items in which the order of the items does not explicitly matter.

You may use any of the following symbols to denote bullets for each list item:

```markdown
* valid bullet
- valid bullet
+ valid bullet
```

For example

```markdown
- Lorem ipsum dolor sit amet
- Consectetur adipiscing elit
- Integer molestie lorem at massa
- Facilisis in pretium nisl aliquet
- Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem
```
Renders to:
<div class="md-rendered-html" style="width:300px;" >
<ul style="margin:0px;">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
</div>

And this HTML

```html
<ul>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
```

### Ordered

A list of items in which the order of items does explicitly matter.

```markdown
1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
   1. Facilisis in pretium nisl aliquet
   2. Nulla volutpat aliquam velit
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem
```
Renders to:

<div class="md-rendered-html" style="width:300px;" >
<ol style="margin:0px;">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <ol>
    <li>Facilisis in pretium nisl aliquet</li>
    <li>Nulla volutpat aliquam velit</li>
  </ol>  
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ol>
</div>

And this HTML:

```html
<ol>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <ol>
    <li>Facilisis in pretium nisl aliquet</li>
    <li>Nulla volutpat aliquam velit</li>
  </ol>  
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ol>
```

**TIP**: If you just use `1.` for each number, Markdown will automatically number each item. For example:

```markdown
1. Lorem ipsum dolor sit amet
1. Consectetur adipiscing elit
1. Integer molestie lorem at massa
1. Facilisis in pretium nisl aliquet
1. Nulla volutpat aliquam velit
1. Faucibus porta lacus fringilla vel
1. Aenean sit amet erat nunc
1. Eget porttitor lorem
```

Renders to:
<div class="md-rendered-html" style="width:300px;" >
<ol style="margin:0px;">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit</li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ol>
</div>

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Code

### Inline code
Wrap inline snippets of code with `` ` ``.

```markdown
In this example, `<section></section>` should be wrapped as **code**.
```

Renders to:
<div class="md-rendered-html" style="width:555px;">
In this example, <code>&lt;section&gt;&lt;/section&gt;</code> should be wrapped with <strong>code</strong>.
</div>

HTML:

```html
<p>In this example, <code>&lt;section&gt;&lt;/section&gt;</code> should be wrapped with <strong>code</strong>.</p>
```

### Indented code

Or indent several lines of code by at least four spaces, as in:

```markdown
// Some comments
line 1 of code
line 2 of code
line 3 of code
```
Renders to:
<div class="md-rendered-html" style="width:200px;">
<code>
  <pre style="padding: 0 0 0 0; margin: -20px 0 -45px -35px;">
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
    </pre>
  </code>
</div>

HTML:

```html
<pre>
  <code>
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
  </code>
</pre>
```
### Block code "fences"

Use "fences"  ```` ``` ```` to block in multiple lines of code.

<pre>
``` markup
Sample text here...
```
</pre>

```
Sample text here...
```

HTML:

```html
<pre>
  <code>Sample text here...</code>
</pre>
```

### Syntax highlighting

GFM, or "GitHub Flavored Markdown" also supports syntax highlighting. To activate it, simply add the file extension of the language you want to use directly after the first code "fence", ` ```js `, and syntax highlighting will automatically be applied in the rendered HTML. For example, to apply syntax highlighting to JavaScript code:

<pre>
```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```
</pre>
<div style="margin-top:-20px;"></div><!-- needed sometimes -->

Renders to:

```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```
<!-- ------------------------------------------------------------------------------------------------------------ -->

## Links

### Basic link
<br> 

```markdown
[Assemble](http://assemble.io)
```  

Renders to (hover over the link, there is no tooltip):
<div style="margin-top:-20px;"></div>

[Assemble](http://assemble.io)

HTML:

```html
<a href="http://assemble.io">Assemble</a>
```

### Add a title  
<div style="margin-top:20px;"></div><!-- needed somtimes -->

```markdown
[Upstage](https://github.com/upstage/ "Visit Upstage!")
```

Renders to (hover over the link, there should be a tooltip):
<div style="margin-top:-20px;"></div>

[Upstage](https://github.com/upstage/ "Visit Upstage!")

HTML:

```html
<a href="https://github.com/upstage/" title="Visit Upstage!">Upstage</a>
```

### Named Anchors

Named anchors enable you to jump to the specified anchor point on the same page. For example, each of these chapters:

```markdown
# Table of Contents
  * [Chapter 1](#chapter-1)
  * [Chapter 2](#chapter-2)
  * [Chapter 3](#chapter-3)
```
will jump to these sections:

```markdown
## Chapter 1 <a id="chapter-1"></a>
Content for chapter one.

## Chapter 2 <a id="chapter-2"></a>
Content for chapter one.

## Chapter 3 <a id="chapter-3"></a>
Content for chapter one.
```
**NOTE** that specific placement of the anchor tag seems to be arbitrary. They are placed inline here since it seems to be unobtrusive, and it works.

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Images
Images have a similar syntax to links but include a preceding exclamation point.

```markdown
![Minion](https://octodex.github.com/images/minion.png)
<img src="https://octodex.github.com/images/minion.png" width="250px">

```
<!-- ![Minion](https://octodex.github.com/images/minion.png) -->
<img src="https://octodex.github.com/images/minion.png" width="250px">

and using a local image (which also displays in GitHub):

```markdown
![Octocat](assets/images/octocat.jpg)
<img  src="assets/images/octocat.jpg" width="250px">
```

<!-- ![Octocat](assets/images/octocat.jpg) -->

<img src="assets/images/octocat.jpg" width="250px">

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Emphasis

### Bold
For emphasizing a snippet of text with a heavier font-weight.

The following snippet of text is **rendered as bold text**.

```markdown
**rendered as bold text**
```
renders to:
<div class="md-rendered-html" style="width: 200px; padding: 0px 0px 4px 10px;">
<strong>rendered as bold text</strong>
</div>

and this HTML

```html
<strong>rendered as bold text</strong>
```

### Italics
For emphasizing a snippet of text with italics.

The following snippet of text is _rendered as italicized text_.

```markdown
_rendered as italicized text_
```

renders to:
<div class="md-rendered-html" style="width: 220px; padding: 0px 0px 4px 10px;">
<em>rendered as italicized text</em>_
</div>

and this HTML:

```html
<em>rendered as italicized text</em>
```

### strikethrough
In GFM (GitHub flavored Markdown) you can do strikethroughs.

```markdown
~~Strike through this text.~~
```
Which renders to:
<div class="md-rendered-html" style="width: 190px; padding: 0px 0px 4px 10px;">
<del>Strike through this text.</del>
</div>

HTML:

```html
<del>Strike through this text.</del>
```
<!-- ------------------------------------------------------------------------------------------------------------ -->

## Comments

Comments should be HTML compatible
```html
<!--
This is a comment
-->
```

Comment below should **NOT** be seen:
<div class="md-rendered-html" style="height:80px; width:300px;" >
<!--
This is a comment
-->
</div>

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Blockquotes
For quoting blocks of content from another source within your document.

Add `>` before any text you want to quote.

```markdown
> **Fusion Drive** combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.
```
Renders to:
<div class="md-rendered-html" style="width:100%; margin: -17px 0px 0px -25px; padding: 0px 5px 10px 20px;">
<blockquote>
  <p><strong>Fusion Drive</strong> combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.</p>
</blockquote>
</div>

and this HTML:
```html
<blockquote>
  <p><strong>Fusion Drive</strong> combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.</p>
</blockquote>
```

Blockquotes can also be nested:

```markdown
> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
```

Renders to:
<div class="md-rendered-html" style="width:100%; margin: -17px 0px 0px -25px; padding: 0px 5px 10px 20px;">
<blockquote>
  Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
  Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
  <blockquote>
    Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
    odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
  </blockquote>
</blockquote>
</div>

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Horizontal Rules

The HTML `<hr>` element is for creating a "thematic break" between paragraph-level elements. In markdown, you can create a `<hr>` with any of the following:

* `___`: three consecutive underscores
* `---`: three consecutive dashes
* `***`: three consecutive asterisks

renders to:
<div class="md-rendered-html" style="padding: 8px 8px 15px 10px; width:100%;">
    <hr class="md-line">
    <hr class="md-line" style="width:400px; height:4px;">
    <hr class="md-line" style="width:200px; height:6px; background-color:red;">
</div>    

<!-- ------------------------------------------------------------------------------------------------------------ -->

## Tables

Tables are created by adding pipes as dividers between each cell, and by adding a line of dashes (also separated by bars) beneath the header. Note that the pipes do not need to be vertically aligned.


```markdown
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

Renders to:

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

And this HTML:

```html
<table>
  <tr>
    <th>Option</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>data</td>
    <td>path to data files to supply the data that will be passed into templates.</td>
  </tr>
  <tr>
    <td>engine</td>
    <td>engine to be used for processing templates. Handlebars is the default.</td>
  </tr>
  <tr>
    <td>ext</td>
    <td>extension to be used for dest files.</td>
  </tr>
</table>
```

### Right aligned text

Adding a colon on the right side of the dashes below any heading will right align text for that column.

```markdown
| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

<!-- ------------------------------------------------------------------------------------------------------------ -->

> Note: Example page content from [GetGrav.org](https://learn.getgrav.org/17/content/markdown), included to demonstrate the portability of Markdown-based content
