

# HMTL
**You need**
- Google Chrome, you can also use another network but the recomendation is this one
- Visual Studio Code, better if you dont use Netbeans

**You download extensions**
- vscode-icons= better image
- prettier = code formatter
- live server = little server you can load changes in html automatic

## Website Theory
**Who work?**
- Frontedn: user can see
- Backend: Code, the user cant see it, write and read data, etc
**Roles**
- Frontend Developer
- Backend Developer
- Fullstack Developer (Frontend + Backend)
**Languages**
- HTML
- CSS
- JS (Javascript)

**Network Traffic**
- Client Request to server
- Server Response to client
## Basic Structure

```html
<!DOCTYPE html> <!--elemento> version </elemento>--> 
<html> 
<head> <!--elemento> meta data web description </elemento>-->
<title> Mi Primer Proyecto</title> <!--elemento> name </elemento>-->
</head>
<body>

</body>
</html> 
```

## Head
A option to use head is to load files (you can also do the same action in body), but in head is the first that is going to load in the project, is an advantage if you have a heavy Javascript project.
If you press ! and enter you automatically you have HTML structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"><!--e> mention data set of characters that you use </e>-->
    <meta http-equiv="X-UA-Compatible" content="IE=edge"> <!--e> the content is friendly to internet explorer </e>-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"><!--e> window size </e>-->
    <title>Mi primer proyecto</title>
</head>
<body>
    
</body>
</html> 
```
## Images

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primer proyecto</title>
</head>
<body>
    <img src= "imagenes/foto.png" alt="imagen de Boo"/> <!--e> src= where find the image, alt= if you lose the image </e>-->
</body>
</html>
```
## CSS Basics 1
There us 3 ways to implamate CSS
1. Inline Style: CSS Code writing in one speficied element. (No Recommended)
2. In Style: Inside of HTML's Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primer proyecto</title>
    <!--e>In p (selector elemento cambio)</e-->
    <style> 
        p {
            color:pink;

        }
    </style>
</head>
<body>
    <img src= "imagenes/foto.png" alt="imagen de Boo"/>
    <p style = "color:blue">Hola me llamo Monica</p> <!--e>Inline</e-->
</body>
</html>
```
3. External CSS: Create another CSS file (.css)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primer proyecto</title>
    <link rel="stylesheet" href="index.css"/>  <!--e>rel= archivo href=ubicacion</e-->
</head>
<body>
    <img src= "imagenes/foto.png" alt="imagen de Boo"/>
    <p>Hola me llamo Monica</p> 
</body>
</html>
```
```css
p{
    color:aqua;
    font-size:30px ;
}
```