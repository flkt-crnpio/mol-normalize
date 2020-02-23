## mol normalize
normalize css file a.k.a. para que se vean igual las etiquetas de html en todos los navegadores. tiene unas pocas variables para poder editar el estilo general como el color primario o la tipografía y media queries para cambiar el tamaño de los títulos.

### scripts
* para obtener el archivo minificado `npm run mol`
* para ver los cambios locales `npm run dev`

### variables
```text
$m-font-family: sans-serif;
$m-font-size: 16px;
$m-font-weight: 400;
$m-letter-spacing: normal;
$m-line-height: 1.5em;

$m-code-family: monospace;

$m-em-family: serif;

$m-h-family: sans-serif;
$m-h-size: 23px;
$m-h-height: 1em;
$m-h-spacing: normal;
$m-h-weight: 600;
$m-h-style: normal;
$m-h-transform: none;

$m-colors: (
  "background": #FFF,
  "font": #292321,
  "primary": #19efaf
);

$m-queries: (
  "phone": (
    "since": 320px,
    "until": 767px,
  ),
  "tablet": (
    "since": 768px,
    "until": 1024px,
  ),
  "laptop": (
    "since": 1025px,
    "until": 1599.99px,
  ),
  "desktops": (
    "since": 1600px,
    "until": 99999px,
  )
);
```

### archivos
```text
mol-n/
├── mol/
│   ├── n.min.css
│   └── n.min.css.map
├── dev/
│   ├── index.html
│   ├── n.css
│   └── n.css.map
└── scss/
    ├── _normalize.scss
    ├── _vars.scss
    └── n.scss
```

## problemas conocidos

(//▽//) El input type search funciona como un input type text, para mantener el estilo general de los inputs
