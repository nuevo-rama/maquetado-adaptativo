# maquetado-adaptativo-responsive-media-queries

#### Maquetado web Adaptativo - Responsive
#### Media Queries

- html
- css

## Pasos para generar el inicio de un maquetado adaptativo - responsive
----

1. Creo el repositorio en Github 
2. ```git bash here```
3. ```git clone [url]```
4. ```code .```
5. Creo el archivo app.js (entry point)
6. En VS ```npm init```
7. ```npm install```
8. En terminal creo el archivo ```.gitignore``` y escribo ```node_modules/``` (no se hace el push de lo que está en gitignore al repositorio)
9. Creo la estructura de carpetas
10. En la carpeta Views creo el archivo index.html
11. Agrego el campo para maquetado adaptativo en el head ```<meta name="viewport" content="width=device-width, initial-scale=1">```
12. ```git add .```
13. ```git commit -m "mensaje"```
14. ```git push```

----

## En la hoja de estilos CSS aplicamos **media-queries**


```css
@media (min-width: 460px) {
  body {
  background: red;
  }
}
```

#### Ese código dice que:

- Si como **mínimo** el viewport tiene x cantidad de píxeles, entonces apliquemos las siguientes reglas.

-----

```css
@media (max-width: 768px) {
  body {
  background: green;
  }
}
```

#### Ese código dice que:

- Si como **máximo** el viewport tiene x cantidad de píxeles, entonces apliquemos las siguientes reglas.

-----

```css
@media (max-width: 768px) and (orientatios: landscape) {
  body {
  background: blue;
  }
}
```

#### Ese código dice que:

- Si como **máximo** el viewport tiene x cantidad de píxeles y además el dispositivo está en posición (vertical/horizontal), entonces apliquemos las siguientes reglas.

-----

Lo ideal es utilizar la regla **MOBILE FIRST**.
Que irá al final de la hoja de estilos.

```css
@media (min-width: 460px) {
  /*TABLETS*/
}

@media (min-width: 768px) {
  /*LAPTOPS*/
}
```

------

# LAS MEDIDAS DE LOS DISPOSITIVOS

- SMALLER SMARTPHONES 0-480 px
- TABLETS AND LARGER SMARTPHONES 481-768
- LAPTOPS, LARGER SMARTPHONES IN LANDSCAPE AND SMALL DESKTOPS 769-1279
- LARGER DESKTOPS AND MONITORS +1280





