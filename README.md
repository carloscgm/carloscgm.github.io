# carloscgm.github.io

Páginas públicas de las apps de carloscgm: políticas de privacidad y ayuda. Se publican con GitHub Pages en https://carloscgm.github.io.

## Estructura

Cada app va en su propia carpeta, con sus páginas en cada idioma:

```
index.html          lista de apps
leve/
  privacy.html      redirige al idioma del navegador
  support.html
  es/ en/ pt-br/ fr/ de/ it/
```

Direcciones de Leve para las tiendas:

- Política de privacidad: https://carloscgm.github.io/leve/privacy.html
- Soporte: https://carloscgm.github.io/leve/support.html

## No se edita aquí

Las páginas de cada app se generan en el repositorio de la app y se copian a su carpeta. Para Leve, desde `photo_swapper`:

```
python3 tool/site/build_site.py
tool/site/publish_site.sh ../carloscgm.github.io
```

Luego, aquí: revisar el cambio, hacer commit y push. GitHub Pages lo publica en uno o dos minutos.

## Añadir otra app

1. Que la app genere sus páginas en una carpeta propia, con enlaces relativos.
2. Copiarlas a `<app>/` en este repositorio.
3. Añadirla a la lista de `index.html`.

Las direcciones de cada app no deben cambiar después de publicarla: las tiendas las guardan.
