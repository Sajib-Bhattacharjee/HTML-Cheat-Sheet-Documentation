# HTML Cheat-Sheet

In detail all about the topic.

## Table of Contents

- [1.Introduction/Overview](#1introduction)
- [2.Head](#2head)
- [3.Text content](#3text-content)
  - [3.1-Headings](#headings)
  - [3.2-Paragraphs](#paragraphs)
  - [3.3-Formatting](#formatting)
  - [3.4-Quotes](#quotes)
- [4.Content](#4content)
  - [4.1-Links](#links)
  - [4.2-Images](#images)
  - [4.3-Blocks](#blocks)
- [5.Lists](#5lists)
  - [5.1-Unordered list](#unordered-list)
  - [5.2-Ordered list](#ordered-list)
  - [5.3-Definition list](#definition-list)
- [6.Tables](#6tables)
  - [6.1-Basic table](#basic-table)
  - [6.2-Accessible table/Advanced table](#advanced-table)
- [7.Forms](#7forms)
- [8.HTML5 Semantic Tags](#8html5-semantic-tags)
  - [8.1-HTML Page layout](#page-layout)
  - [8.2-More Semantic Tag](#more-semantic-tags)
  - [8.3-Semantic Media Tags](#semantic-media-tags)
- [9.Emojis](#9emojis)

## 1.Introduction

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Title( Example- Dedicated For "Zahan")</title>
  </head>
  <body>
    <!-- content here -->
  </body>
</html>
```

## 2.Head

```html
<head>
  <title>Title( Example- Dedicated For "Zahan")</title>
  <base href="base-url" />
  <link href="style.css" rel="stylesheet" type="text/css" />
  <style type="text/css">
    /* CSS code */
  </style>
  <script src="script.js"></script>
  <script>
    // Javascript code
  </script>
  <meta charset="UTF-8" />
  <meta name="keywords" content="keywords" />
  <meta name="description" content="description" />
  <meta name="author" content="name" />
  <meta http-equiv="refresh" content="10" />
</head>
```

| tag                                            | element                  |
| ---------------------------------------------- | ------------------------ |
| **title**                                      | page title               |
| **base**                                       | base url for all links   |
| **link**                                       | link to external source  |
| **style**                                      | CSS inside HTML page     |
| **script**                                     | Javascript code          |
| **meta**                                       | metadata                 |
| **meta** _http-equiv_="refresh" _content_="10" | auto-refresh page in 10s |

## 3.Text content

### Headings

```html
<h1>Main heading</h1>
<!-- etc -->
<h6>Level-6 heading</h6>
```

| tag    | element                 |
| ------ | ----------------------- |
| **h1** | main heading            |
| **h6** | least important heading |

### Paragraphs

```html
<p>
  Paragraph.<br />
  Other line.
</p>
<p>Other paragraph.</p>
<hr />
<p>See the line above.</p>
```

| tag    | element         |
| ------ | --------------- |
| **p**  | paragraph       |
| **br** | line break      |
| **hr** | horizontal line |

### Formatting

```html
<em>Formatting</em> is <strong>important</strong> ! (a+b)<sup>2</sup> = a<sup
  >2</sup
>
+ b<sup>2</sup> + 2ab
```

| tag        | element     |
| ---------- | ----------- |
| **sub**    | subscript   |
| **sup**    | superscript |
| **em**     | emphasize   |
| **strong** | important   |
| **mark**   | highlighted |
| **small**  | small       |
| **i**      | italic      |
| **b**      | bold        |

### Quotes

```html
<cite>This book</cite> was written by this author.
<q cite="url">quotation</q>
<blockquote cite="url">
  Lorem ipsum<br />
  Lorem ipsum
</blockquote>
```

| tag            | element          |
| -------------- | ---------------- |
| **cite**       | title of a work  |
| **q**          | inline quotation |
| **blockquote** | quotation        |

## 4.Content

### Links

```html
<a href="url">link</a>
<a href="url" target="_blank">open in a new window</a>

<a href="#comments">watch comments</a>
<h2 id="comments">comments</h2>
```

| tag   | element   |
| ----- | --------- |
| **a** | hyperlink |

### Images

```html
<img src="image.png" alt="description" width="300" height="200" />
```

| tag     | element |
| ------- | ------- |
| **img** | image   |

### Blocks

```html
<div>block</div>
<span>inline</span>
```

| tag      | element             |
| -------- | ------------------- |
| **div**  | block-level element |
| **span** | inline element      |

## 5.Lists

### Unordered list

```html
<ul>
  <li>item</li>
  <li>item</li>
  <li>item</li>
</ul>
```

| tag    | element        |
| ------ | -------------- |
| **ul** | unordered list |
| **li** | list item      |

### Ordored list

```html
<ol>
  <li>first</li>
  <li>second</li>
  <li>third</li>
</ol>
```

| tag    | element      |
| ------ | ------------ |
| **ol** | ordered list |
| **li** | list item    |

### Definition list

```html
<dl>
  <dt>term</dt>
  <dd>definition</dd>
  <dt>term</dt>
  <dd>definition</dd>
  <dt>term</dt>
  <dd>definition</dd>
</dl>
```

| tag    | element         |
| ------ | --------------- |
| **dl** | definition list |
| **dt** | term            |
| **dd** | definition      |

## 6.Tables

### Basic table

```html
<table>
  <tr>
    <th>heading 1</th>
    <th>heading 2</th>
  </tr>
  <tr>
    <td>line 1, column 1</td>
    <td>line 1, column 2</td>
  </tr>
  <tr>
    <td>line 2, column 1</td>
    <td>line 2, column 2</td>
  </tr>
</table>
```

| tag       | element       |
| --------- | ------------- |
| **table** | table         |
| **tr**    | table row     |
| **th**    | table heading |
| **td**    | table cell    |

### Accessible Table

```html
<table>
  <caption>
    caption
  </caption>
  <colgroup>
    <col span="2" style="..." />
    <col style="..." />
  </colgroup>
  <thead>
    <tr>
      <th>heading 1</th>
      <th>heading 2</th>
      <th>heading 3</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <th>footer 1</th>
      <th>footer 2</th>
      <th>footer 3</th>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>line 1, column 1</td>
      <td>line 1, column 2</td>
      <td>line 1, column 3</td>
    </tr>
    <tr>
      <td>line 2, column 1</td>
      <td>line 2, column 2</td>
      <td>line 2, column 3</td>
    </tr>
  </tbody>
</table>
```

| tag          | element                     |
| ------------ | --------------------------- |
| **caption**  | caption                     |
| **colgroup** | defines groups of columns   |
| **col**      | defines column's properties |
| **thead**    | groups headings together    |
| **tfoot**    | groups footers together     |
| **tbody**    | groups other rows           |

## 7.Forms

```html
<form action="url" method="post">
    <fieldset>
        <legend>Who are you ?</legend>
        <label>Login :<input type="text" name="login" /></label><br/>
        <label for="pswd">Password :</label><input type="password" name="password" id="pswd" /><br/>
        <input type="radio" name="sex" value="male" />Male<br/>
        <input type="radio" name="sex" value="female" />Female<br/>
    </fieldset>

    <label>Your favorite color : <select name="color">
        <option>red</option>
        <option>green</option>
        <option>blue</option>
    </select></label>

    <input type="checkbox" name="available" value="monday" />Monday<br/>
    <input type="checkbox" name="available" value="tuesday" />Tuesday<br/>

    <textarea name="comments" rows="10" cols="30" placeholder="Write your comments here"><textarea/>

    <input type="submit" value="Button text">
</form>
```

| tag                         | element                       |
| --------------------------- | ----------------------------- |
| **form**                    | form                          |
| **label**                   | label for input               |
| **fieldset**                | group inputs together         |
| **legend**                  | legend for fieldset           |
| **input** type="_text_"     | text input                    |
| **input** type="_password_" | password input                |
| **input** type="_radio_"    | radio button                  |
| **input** type="_checkbox_" | checkbox                      |
| **input** type="_submit_"   | send form                     |
| **select**                  | drop-down list                |
| **option**                  | drop-down list item           |
| **optgroup**                | group of drop-down list items |
| **datalist**                | autocompletion list           |
| **textarea**                | large text input              |

## 8.HTML5 Semantic Tags

### Page layout

```html
<header>My website</header>
<nav>
  <a href="page1">Page 1</a>
  <a href="page2">Page 2</a>
  <a href="page3">Page 3</a>
</nav>

<section>Hello everybody, Welcome to my website !</section>

<article>
  <header>
    <h2>Title( Example- Dedicated For "Zahan")</h2>
  </header>
  <p>My article</p>
</article>

<aside>Writen by me</aside>

<section id="comments">
  <article>Comment 1</article>
  <article>Comment 2</article>
</section>

<footer>Copyright notice</footer>
```

| tag         | element                                      |
| ----------- | -------------------------------------------- |
| **header**  | header of document or section                |
| **footer**  | footer of document or section                |
| **section** | section                                      |
| **article** | article, forum post, blog post, comment      |
| **aside**   | aside content related to surrounding content |
| **nav**     | navigation links                             |

### More Semantic Tags

```html
<figure>
  <img src="image.png" alt="figure 1" />
  <figcaption>Figure 1</figcaption>
</figure>

<details>
  <summary>
    Declaration of M. X on <time datetime="2013-12-25">Christmas day</time>
  </summary>
  <p>M. X said...</p>
</details>

Downloading progress : <progress value="53" max="100"></progress> Disk space :
<meter value="62" min="10" max="350"></meter>
```

| tag            | element                              |
| -------------- | ------------------------------------ |
| **figure**     | an illustration                      |
| **figcaption** | caption of a figure element          |
| **details**    | details that can be shown or hidden  |
| **summary**    | visible heading of a details element |
| **progress**   | progress of a task                   |
| **meter**      | display a gauge                      |
| **time**       | machine-readable time indication     |

### Semantic Media Tags

````html
<figure></figure> Embeds annotated images, illustrations, photos, code, etc.
<figcaption></figcaption> For adding a caption/annotation to the <figure>.
<picture></picture> Responsive image insertion,allows developers to provide different images for different contexts.

<video poster=" " autoplay loop controls ></video>For embedding videos into a website.
   poster is the path to an image that’s displayed before the video plays.
   autoplay will start the video automatically.
   loop triggers whether the video should repeat or not.
   controls shows or hides the browser’s player buttons.

<audio></audio> For embedding audio into a website.
<source></source> Must be inside <picture>, <video> or <audio> to define the different versions of content.
```
````

## 9.Emojis

```html
<p style="font-size:48px">&#128512; &#128516; &#128525; &#128151;</p>
```

Output:

<p style="font-size:48px">&#128512; &#128516; &#128525; &#128151;</p>

> For Emoji Unicode refer _[This Website(w3schools)](https://www.w3schools.com/charsets/ref_emoji.asp)_.

### Created By

`-Sajib Bhattacharjee`

`Dedicated for "Zahan"`

### Thanks A Lot For Visiting...!!!
