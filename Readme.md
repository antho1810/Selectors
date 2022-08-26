**Especificidad y Cascada**
La especificidad tiene mas importante que la cascada. 
Cascada: si se esta poniendo estilos una sola etiqueta se va a tomar la segunda opcion has puesto.
Especifidad es que las etiquedas, atributos, ID, clases estas tiene un nivel de jerarquia diferente
para poner estilos; los selectores ID tiene mas primoridad, los que le siguen son los selectores de 
clase, atributos y pseudoclases, y por ultimo los selectores de tipo y pseudoelementos. 


**BEM(Block Element Modifier)**
Es una metodologia que nos proporciona una manera de nombrar a nuestras clases en HTML para posteriormente poder usarlo en CSSm BEM nos ayudara a mantener nuestro código flexible, modular y sencillo. Sobre todo a lidiar con problemas sobre especifidad.
BEM significa Block Element Modifier, esto es debido a que todas las clases que escribiremos se regiran por estas 3 partes.

**Block**
Es una parte independiente en nuestro HTML, no necesita de otros elementos para existir. Por ejemplo, una galeria de imágenes o un menú, no necesita de otros elementos para existir.

Los bloques tienen el nombre de lo que representará, ejemplo "header, menu, galeria, foooter"

```
<section class="gallery">

</section>
```

**Element**
Un elemento siempre estara dentro de un bloque, debido a que es parte de él y es dependiente del bloque, por ejemplo una imágen necesita una galería de imagenes para existir, o un enlace necesita un menu para existir.

Los elementos tendran el nombre primero de el boque al que pertenece, 2 guiones bajos y despues el nombre de lo que representará un ejmplo: "header__title, meny__item, galeria__img, footer__img"

```
<section class="gallery">
 <img src="" class="gallery__img" />
</section>
```

**Modifier**
Los modficadores son usados en elementos o bloques, se usan para representar una caracteristica diferente que tendrá el modificador o elemento.

Los modficadores tendrán el nombre del bloque o del elemento, despues otra vez el nombre del elemento, dos guiones medios y la caracteristica diferente que tendrá este bloque o elemento.

Ejemplo: "boton--active""header--wave"

```
<button class="btn">Dame click</button>
<button class="btn">Dame click</button>
<button class="btn btn--active">Dame click</button>
```
