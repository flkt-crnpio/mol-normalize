# mol normalize

(≧ ▽ ≦)ノ weeeenaaaaaaas!!!

este proyecto es para normalizar los elementos nativos de HTML entre distintos navegadores a la vez que sirve de base para proyectos pequeños.

se pueden configurar los estilos directamente con el uso de propiedades personalizadas (variables) de CSS, que actúan directamente sobre las etiquetas nativas sin necesidad de escribir ninguna clase a ningún elemento.

y pesa tan solo 12 KB en disco!

**llame ya!**

*( no llamen... nunca contesto )*

## uso

＼(￣▽￣)／ no se necesita volver a compilar! 

simplemente utiliza el archivo minificado y con las propiedades de CSS puedes variar el resultado tanto en modo claro como oscuro.

### --variables-de-color

solamente tiene tres variables de color, una para el fondo general, otra para el texto y un color primario para los elementos interactivos. Para que funcione correctamente, se requiere que tanto el texto como el color primario tengan suficiente contraste contra el fondo.

los elementos que tienen color están mezclados con el color primario para darle homogeneidad a la paleta de tonalidades.

```scss
// variables css color tema oscuro
:root {
  --m-color-fondo: rgb(18, 14, 24);
  --m-color-texto: rgb(255, 255, 255);
  --m-color-primario: rgb(0, 255, 187);
}

// variables css color tema claro
@media (prefers-color-scheme: light) {
  :root {
    --m-color-texto: rgb(18, 14, 24);
    --m-color-fondo: rgb(255, 255, 255);
    --m-color-primario: rgb(74, 34, 255);
  }
}
```

### --variables-del-documento

las variables del documento interactúan con múltiples etiquetas, es importante que para el tamaño de texto se utilicen en unidades absolutas, para el interlineado y el espaciado se requieren unidades relativas.

```css
  --m-documento-texto: 18px;
  --m-documento-interlineado: 1.375em;
  --m-documento-espaciado: 1rem;
```

### --variables-de-texto

se pueden utilizar distintas familias tipográficas y estilos para el texto, títulos y código, pero es importante declarar el tamaño del texto para cada caso en unidades relativas.

```css
  --m-texto-tipografia: sans-serif;
  --m-texto-peso: 400;
  
  --m-titulo-tipografia: sans-serif;
  --m-titulo-tamanio: 1rem;
  --m-titulo-interlineado: 1.25em;
  --m-titulo-peso: 500;
  --m-titulo-margen: 1.25em 0 0;

  --m-codigo-tipografia: monospace;
  --m-codigo-peso: 400;
  --m-codigo-tamanio: 0.9em;
  --m-codigo-espaciado: 0.025em;
```

### --variables-de-formularios

por último, con estas variables se pueden configurar un poco los estilos en los formularios y elementos interactivos.

```css
  --m-formulario-borde-tamanio: 1px;
  --m-formulario-borde-estilo: solid;
  --m-formulario-redondeado: 3px;
  --m-formulario-espaciado: var(--m-documento-espaciado);

  --m-campo-altura: 44px;
  --m-campo-borde-tamanio: 1px;
  --m-campo-borde-estilo: solid;
  --m-campo-espaciado: .5em;
  --m-campo-redondeado: 3px;
  
  --m-boton-borde-tamanio: 0;
  --m-boton-borde-estilo: solid;
  --m-boton-espaciado: .5em 1em;
  --m-boton-redondeado: 999rem;

  --m-enfoque-borde-estilo: solid;
  --m-enfoque-borde-tamanio: 4px;
  --m-enfoque-espaciado: 2px;
```

## notas

(っ´ω`)ﾉ(╥ω╥) los inputs de type range, checkbox y radio, se muestran tal cual los presenta cada navegador. No se alteró su estilo porque para lograr homologarlos es necesario el uso de otros elementos y/o tecnologías.

## 

 	( . .)φ__  flkt.crnpio@gmail.com
