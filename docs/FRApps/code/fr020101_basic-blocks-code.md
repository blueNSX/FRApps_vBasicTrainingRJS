<!-- ---------------------------------------------------------------------- -->
<div class="page-back">

[<-- BACK](/FRApps/fr020101_Basic-Blocks)

</div><div class="page-next">

<!-- ---------------------------------------------------------------------- -->

HTML

___


```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
       <meta charset="UTF-8">
       <meta http-equiv="X-UA-Compatible" content="ie=edge">
       <link rel="stylesheet" href="index.css">
       <link rel="shortcut icon" href="../favicon.gif">
       <title>FRApps Basic Blocks</title>
    </head>
    <body>
        <div class="header">
            <h2>header</h2>
        </div>
        <div class="section1">
           <h2>section 1</h2>
        </div>
        <div class="section2">
            <h2>section 2</h2>
        </div>
        <div class="footer">
            <h2>footer</h2>
        </div>
    </body>
</html>
```


CSS

___


```css
/* Basic Blocks */

@import url('https://fonts.googleapis.com/css?family=Bookman Old Style');

/*-----------------------------------------
root selector to create variables
-------------------------------------------*/
:root {
    --header-color: red;
    --section1-color: blue;
    --section2-color: lightgray;
    --footer-color: green;
    --h2-text-color-light: white;
    --h2-text-color-dark: black;
    --nav-list-item-hover-color: white;
    --h2-font-size: 1.5rem;
    --nav-list-font-size: 1.2rem;
    --footer-list-font-size: .9rem;
} 

/*-----------------------------------------
The html properites
------------------------------------------*/
html {
    background: #b3b3b3;
    height: 100%;
    text-align: center;
}

/*-----------------------------------------
The body properites
------------------------------------------*/
body {
    background: white;
    height: 100%;
}

/*-----------------------------------------
Set global properties for the <h2> tags
It also overrides the intrinsic margin of
20 to 0--allowing to stack the blocks together
-------------------------------------------*/
h2 {
    margin: 0;
    font-size: var(--h2-font-size) ;
    color: var(--h2-text-color-light);
    padding: 1.5rem;
    text-align: center;
  }

/*-----------------------------------------
The .header properites
------------------------------------------*/
.header {
    background: var(--header-color);
    width: 300px;
    height: 100px;
    position: relative;
}

/*-----------------------------------------
The .section1 properites
------------------------------------------*/
.section1 {
    background: var(--section1-color);
    width: 300px;
    height: 100px;
    position: relative;
}

/*-----------------------------------------
The .section2 properites
------------------------------------------*/
.section2 {
    background: var(--section2-color);
    width: 300px;
    height: 100px;
    position: relative;
}

/*-----------------------------------------
This is another <h2> override
setting the font color from white to black
------------------------------------------*/
.section2 h2 {
    color: var(--h2-text-color-dark);
}

/*-----------------------------------------
The .footer properites
------------------------------------------*/
.footer {
    background: var(--footer-color);
    width: 300px;
    height: 100px;
    position: relative;
}

```
___