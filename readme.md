## HTML/CSS CLEAN CODE RULE

### #1. Keep it DRY (`Don't Repeat Yourself`)
Remove the duplication of code using `CSS Rule` and `SASS Rule`

#### CSS Rule
- `Grouping`

Button duplication of code
```css
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
Clean code by `grouping`
```css
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
#### A. Long selector
```css
/* Not recommended */
body .container .card li { .... }
```
```css
/* Recommended */
.card li { .... }
```
#### B. Group selector
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
### HTML
#### 1. Capitalization (`Use only lowercase`)
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
#### 2. Use meta tags