## HTML/CSS CLEAN CODE RULE

### HTML

#### A. Meta tags
```html
<!-- Use for support any language on your website -->
<head>
  <meta charset="UTF-8">
</head>
```
```html
<!-- Use for responsive on your website -->
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
```
```html
<!-- Use for SEO on your website -->
<head>
  <meta name="description" content="Free tutorials">
  <meta name="keywords" content="HTML, CSS, Clean code">
  <meta name="author" content="Rady Y">
</head>
```

#### B. Capitalization (`Use only lowercase`)
```html
<!-- Not recommended -->
<INPUT TYPE="TEXT" PLACEHOLDER="ENTER">
```
```html
<!-- Recommended -->
<input type="text" placeholder="Enter">
```
```css
/* Not recommended */
color: #4EECDE;
```
```css
/* Recommended */
color: #4eecde;
```
#### C. Class name
```html
<!-- Not recommended -->
<div class="rady">
    <div class="ww-left"></div>
    <div class="my33-center"></div>
    <div class="my-right"></div>
</div>
```
```html
<!-- Recommended -->
<div class="container">
    <div class="sidebar-left"></div>
    <div class="main-content"></div>
    <div class="sidebar-right"></div>
</div>
```
### CSS

#### A. Use `CSS Universal selector`
```css
/* Not recommend */
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    background-color: blue;
}
ul a {
    text-decoration: none;
    color: #fff;
}
button {
    border:none;
    background-color: red;
    cursor: pointer;
    width: 100%;
}
h1, p {
    margin: 0;
    padding: 0;
    font-family: "Sans-Serif";
    text-align: center;
}
```
```css
/* Recommend */
* {
    margin: 0;
    padding: 0;
    border:none;
    text-decoration: none;
    box-sizing: border-box;
    font-family: "Sans-Serif";
}
ul {
   background-color:blue;
}
ul a {
    color: #fff;
}
button {
    background-color: red;
    cursor: pointer;
    width: 100%;
}
h1, p {
   text-align: center;
}
```
#### B. Use `Grouping`

```css
/* Not recommended */
.btn-primary {
    cursor: pointer;
    background: blue;
    border:none;
    padding:10px;
    color: #fff;
}
.btn-secondary {
    cursor: pointer;
    background: gray;
    border:none;
    padding:10px;
    color: #fff;
}
.btn-danger {
    cursor: pointer;
    background: red;
    border:none;
    padding:10px;
    color: #fff;
}
.btn-warning {
    cursor: pointer;
    background: orange;
    border:none;
    padding:10px;
    color: #fff;
}
```

```css
/* Recommended */
button {
    cursor: pointer;
    border:none;
    padding:10px;
    color: #fff;
}
.btn-primary {
    background: blue;
}
.btn-secondary {
    background: gray;
}
.btn-danger {
    background: red;
}
.btn-warning {
    background: orange;
}
```
#### C. Long selector
```css
/* Not recommended */
body .container .card li { .... }
```
```css
/* Recommended */
.card li { .... }
```
#### D. Group selector
```css
/* Not recommended */
.container, .card , main, footer, header { ... }
```
```css
/* Recommended */
.container,
.card,
main,
footer,
header { ... }
```


### Naming convention
- Camel case: `thisIsMyExample`
```js
// Javascript
let studentName = "";
let hasStudent = false;
let age = 13;
```
```php
// PHP
$studentName = ""
$isFoundA = False
$age = 13
```
```java
// Java
string studentName = "";
boolean hasStudent = false;
int age = 13;
```
- Snake case: `this_is_my_example`
```python
# Python
student_name = ""
has_student = false
age = 13
```
- Kebab case: `this-is-my-example`

```html
<!-- HTML -->
<div class="card">
    <div class="card-header"></div>
    <div class="card-body"></div>
    <div class="card-footer"></div>
</div>
```

```css
/* CSS */
.card {...}
.card-header {...}
.card-body {...}
.card-footer {...}
```