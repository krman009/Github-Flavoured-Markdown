> Demo-repo || Demo of how markdown works in github. (I think !!! :p)

Writing without code will be wrapped in `<p>` tag.

How I've done that Block-code(Inline code)?

```
`<p></p>`
```

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

How?

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```
Remember `<h1>` and `<h2>` gets `border-bottom` automatically.

And all Heading assigned with the `unique-id`.

also works

```
Heading 1
=========
Heading 2
---------
```
<hr />

> Blockquote ? Yes it is.

How?

```
> Blockquote ? Yes it is.
```
<hr />

~~Strikethrough~~

How?

```
~~Strikethrough~~
```
<hr />

* Hi
* How 
* Are 
* You?

How?

```
* Hi
* How 
* Are 
* You?
or 
* Hi
+ How
- Are
* You?
```

**What about ordered list?**

1. One (Hi)
2. Two (How)
3. Three (Are)
4. Four (You)

How?

```
1. One (Hi)
2. Two (How)
3. Three (Are)
4. Four (You)
```

<hr />

*`em` tag*

How?

```
*`em` tag*  OR
_`em` tag_
```

**`strong` tag**

How?

```
**`strong` tag** OR
__`strong` tag__
```

Noticed? Just written inline-code in `em` and `strong` tag.

If you want to produce __\*__ and **\_** then add `\` before `_` and `*`. So `\*` = \* and `\_` = \_

<hr />

**Image:**

![alt text](http://lorempixel.com/100/100/ "title here")

How?

```
![alt text](http://lorempixel.com/output/nature-q-c-100-100-8.jpg "title here")
```

Also works


`![alt text][id]`  
`[id]: http://lorempixel.com/100/100/ "title here"`  

<hr />

**Link:**

[Github](http://github.com "title here")

How?

```
[Github](http://github.com "title here")
```

Also works


`[github][id2]`  
`[id2]: http://github.com "title here"`

<hr />

**Automatic Links? (Yeah)**

http://github.com

How? just paste with the full url means with `http://` or `https://`. e.g. `http://github.com`.

<hr />

You can also use HTML tags.

<table>
  <tr>
    <th> Number </th>
    <th> Name </th>
  </tr>
  <tr>
    <td> 1 </td>
    <td> Kaushalya </td>
  </tr>
</table>

Yes, Table with HTML tags.

> Remember it's **Github Flavoured Markdown**.

<hr />

More code highlighting...

**HTML**

```html
<body>
  <div class="loader"></div>
  <div class="pause">Click To Pause</div>
</body>
```

<hr />

**SASS**

```sass
@import url(http://fonts.googleapis.com/css?family=Karla)
@import url(http://weloveiconfonts.com/api/?family=fontawesome)
@import url(http://weloveiconfonts.com/api/?family=entypo)

 
$color-1: #f9f8f8
$color-2: #ba8978
$color-3: #fb6567
$color-4: #eab8b4
$color-5: #74c4b1
$color-6: #a3645b
$color-7: #cb877a
$color-8: #aba786
$color-9: white


[class*="fontawesome-"]:before
  font-family: 'FontAwesome', sans-serif
  color: darken($color-7, 30%)
  font-size: 1.5em
  position: absolute
  right: 0.4em
  top: 1.70em

[class*="entypo-"]:before 
  font-family: 'entypo', sans-serif
  color: darken($color-9, 30%)
  font-size: 1.5em
  margin: -1.8em 14.5em
  position: absolute
  
[class*="entypo-"]:after
  font-family: 'entypo', sans-serif
  color: darken($color-9, 30%)
  content: '|'
  font-size: 1.8em
  margin: -1.7em 11.7em
  position: absolute

*
  margin: 0
  padding: 0
  @include transition(0.3s all ease-in-out)

body
  background: $color-2
  font-family: 'Karla', sans-serif
  
form 
  width: 24em
  position: absolute
  top: 50%
  left: 50%
  border: 0.2em solid $color-6
  @include border-radius(0.7em)
  margin: -7em 0 0 -10em
  background: $color-1
  overflow: hidden
  @include box-shadow (inset 0 -0.2em 0.2em 0 darken(pink,3%))
  
  &:hover
    @include box-shadow(inset 0 -0.2em 0.1em 0 pink)
  .header
    margin: 1em 0
    padding: 1em
    text-transform: uppercase
    background: $color-3
    color: $color-9
    font-weight: bold  
    text-shadow:  0 0.1em 0.2em #999
    font-size: 1.1em
    border-left: 0.15em solid $color-6
    border-right: 0.15em solid $color-6
    
    a
      float: right  
      color: inherit
      font-size: 0.8em   
      padding: 0.2em 0.4em   
      text-shadow: none not-!important
 
input[type="text"], input[type="password"]
  background: darken($color-9,5%)
  border: 0.1em solid darken($color-9,12%)
  outline: none
  @include border-radius(0.7em)
  font-size: 1.1em 
  width: 17.9em
  margin: 0.3em
  padding: 0.5em 1em
  padding-right: 2.3em
  border-bottom: 0.30em inset darken($color-9,10%)
  color: $color-5
  display: block
  cursor: pointer

::-webkit-input-placeholder
  font-style: italic
  color: darken($color-9,22%)
  font-family: 'Karla', sans-serif

\:-moz-placeholder 
  font-style: italic
  color: darken($color-9,22%)
  font-family: 'Karla', sans-serif

::-moz-placeholder
  font-style: italic
  color: darken($color-9,22%) 
  font-family: 'Karla', sans-serif

\:-ms-input-placeholder 
  font-style: italic
  color: darken($color-9,22%)
  font-family: 'Karla', sans-serif
  
.rem-me
  margin: 1em
  color: darken($color-9,32%) 
  display: inline-block 
  width: 10em

.submit-button
  display: inline-block

input[type="submit"]
  background: linear-gradient(darken($color-9,7%), darken($color-9,14%))
  border: 0.1em solid $color-3
  outline: none
  font-size: 1.2em
  font-weight: bold
  padding: 0.3em 1em
  margin: 0.2em 0 0 2.7em
  text-transform: uppercase
  color: $color-3
  @include border-radius(0.3em)
  cursor: pointer

input[type="submit"]:hover, input[type="submit"]:active
  border-color: $color-5
  
input[type="text"]:hover, input[type="password"]:hover, input[type="text"]:focus, input[type="password"]:focus
  border-color: $color-5

input[type="text"]:focus ~ .entypo-user, input[type="password"]:focus ~ .entypo-key
  opacity: 0

.attribution
  position: absolute
  bottom: 0
  left: 0

  a
    color: $color-9
    text-decoration: none  

.credit
  position: absolute
  right: 0
  top: 0
  
  a
    color: $color-9
    text-decoration: none  

input[type="checkbox"]
  appearance: none
  height: 1.35em
  width: 2.2em
  outline: none
  cursor: pointer
  background: darken($color-9,7%)
  border: 0.1em solid darken($color-9,15%)
  @include border-radius(0.5em)
  overflow: hidden
  position: relative
  
  &:before
    height: 1.3em
    width: 1.1em
    background: $color-3
    position: absolute
    content: ''
    @include transition (all .3s ease-in-out)
    
  &:checked
  
    &:before
      margin: 0 1em
      background: $color-5
      
label[for="remember"]
  margin: 0 0.4em
  margin-top: -0.1em
  position: absolute
  cursor: pointer
```

```scss

$width: 7em;
$height: 3em;
$c-0: #34495e;
$c-1: lighten(#e74c3c,5%);
$c-2: lighten(#e67e22,5%);
$c-3: lighten(#f1c40f,5%); 

label[for="checkbox"] {
  font-size: 2em;
  position: absolute;
  margin-top: 0.2em;
  text-transform: capitalize;
  color: $c-0;
  transition: all 0.5s ease-in-out;
}

input[type="checkbox"] {
  appearance: none;
  width: $width;
  height: $height;
  background: lighten($c-0,25%);
  border-radius: $width / 2;
  position: relative;
  overflow: hidden;
  outline: none;
  transition: all 0.5s ease-in-out;
  
  &:before {
    width: $width / 2;
    height: $height;
    content: '';
    position: absolute;
    background: linear-gradient( lighten($c-1,17%), lighten($c-2,17%), lighten($c-3,17%) );
    transition: all 0.5s ease-in-out;
  }
  &:checked {
    &:before {
      margin: 0 $width / 2;
    }
  
    background: lighten($c-0,35%);
    opacity: 0;
  
    ~label[for="checkbox"] {
      &:before {
        transition: 0.5s all ease-in-out;
        content: '';
        position: absolute;
        height: 0.5em;
        width: 1em;
        margin: -0.1em -2.0em;
        box-shadow:
          0.3em -0.1em 0 $c-0,
          0.3em -0.2em 0 $c-0,
          0.3em -0.1em 0 $c-0;
        background: transparent;
        transform: rotate(120deg);
      }
    }
  }
}
```

<hr />

**CSS**

```css
@import url(http://fonts.googleapis.com/css?family=Source+Code+Pro);

body {
  background: #eee;
}
.logo {
  -webkit-animation-play-state: running !important;
  animation-play-state: running !important;
  font: bolder 4em 'Source Code Pro', sans-serif;
  letter-spacing: -0.12em;
  color: #ddd;
  animation: shadow 2s linear infinite;
  text-shadow: 1px 1px 3px grey, 2px 2px 4px lightgrey, 3px 3px 5px #aaa, 4px 4px 6px #aaa, 5px 5px 6px #bbb, 6px 6px 7px #ccc, 7px 7px 8px #ddd, 8px 8px 9px #eee;
}
@keyframes shadow {
  to {
    text-shadow: 8px 8px 9px #eee, 7px 7px 8px #ddd, 6px 6px 7px #ccc, 5px 5px 6px #bbb, 4px 4px 6px #aaa, 3px 3px 5px #aaa, 2px 2px 4px lightgrey, 1px 1px 3px grey;
    color: grey;
  }
}

```





















