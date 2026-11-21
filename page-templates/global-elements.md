# Global elements template guide
| Name | Selector type | Desctiption |
| --- | --- | --- |
|Global selectors|
|[title](#global-styles) | ID | style settings for titles|
|UI selectors|
|[header](#header) | ID | vertical header CSS & flexbox settings|
|[nav-bar](#navbar)| ID | horizontal navbar CSS & flexbox settings|
|Text box selectors|
|[text-box1](#decorative-content-box-1-deco-box1) | ID | decorated text box|
|MISC|
|[body](#body)| ID | body section divider|
|[organizer-h](#organizer-h)| CLASS | UI organizer for navbar & body|
|[current-page](#misc)| CLASS | navbar current page highlighter|
## Boiler Plate
**HTML**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="styles.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome!!</title>
</head>
```

## Global Styles

**CSS**
```CSS
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');

body {
    font-size: 17px;
    font-family: 'roboto', sans-serif;
    background-color: #0F3D20;
    color: #f5f5dc;
    margin: 0px;
}

#title {
    font-size: 20px;
    font-weight: 600;
}
```
## Header
**HTML**
```HTML
<div id="header">
        <div id="title">openGlade:\\home</div>
</div>
```

**CSS**
```CSS
#header {
    background-color: #1A5E35;
    padding: 10px;
    border-style: groove;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

#header #title {
    background-color: #2D8653;
    padding: 10px;
    border-style: groove;
    border-radius: 25px;
}
```
## Navbar
**HTML**
```HTML
<div id="nav-bar">
            <div>&gt;[Home]</div>
            <div><a href="#">About Me</a>
                <div><a href="#">Journals</a></div>
            </div>
            <div><a href="#">Projects</a>
                <div><a href="#">Photography</a></div>
                <div><a href="#">🍄Mushrooms!!🍄</a></div>
                <div><a href="#">Cookbook</a></div>
            </div>
        </div>
```
**CSS**
```CSS
#nav-bar {
    background-color: #1A5E4F;
    padding: 20px;
    width: 200px;
    border-style: groove;
    border-top-style: none;
    display: flex;
    flex-shrink: 0;
    flex-direction: column;
    min-height: 100vh;
}
#nav-bar a {
    text-decoration: none;
    color: beige;
}
.current-page {
    color: #7DBF82;
}
```
## Body
**HTML**
```HTML
<div id="body">
    ...
    </div>
```
### Decorative Content Box 1 (#deco-box1)
**HTML**
```HTML
    <div id="text-box1">
        <div id="title">Title Here</div>
        <P>Enter paragraph here.</P>
    </div>
```
**CSS**
```CSS
#text-box1 {
    background-color: #7DBF82;
    padding: 10px;
    margin: 20px;
    width: 500px;
    border-style: groove;
    border-radius: 25px;
    display: flex;
    flex-direction: column;
}
```
## MISC
### organizer-h
**HTML**
```HTML
<div class="organizer-h">...</div>
```