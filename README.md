# Recetas Docbook

Este repositorio trata de facilitar la generación de documentación en Docbook. 
## Qué es Docbook

A grandes rasgos Docbook es un lenguaje basado en XML desarrollado para generar documentación. 

El objetivo final es generar documentación sin tener que definir en ningún momento el estilo que se le va a aplicar, de este modo se separa claramente el diseño del contenido

### Ventajas de Docbook
1. Los documento son texto plano, son perfectos para gestionar con un control de versiones
2. Los recursos necesarios para generar documentación son mínimos. Sólo se requiere un editor sencillo
3. Los resultados son muy profesionales
4. El lenguaje no tiene miles de palabras clave con lo que la curva de aprendizaje es rápida
5. Permite convertir a cualquier formato: DOC, PDF, TXT, EPUB...
6. Es un estándar

### Inconvenientes de Docbook
1. Aunque se usa mucho todavía (O'Reilly la usaba para publicar sus libros, FreeBSD, KDE, GNOME desktop documentation, the GTK+ API references, the Linux kernel documentation, The Linux Documentation Project...) es difícil encontrar información para un usuario medio
2. Hay que trabajarse los entornos para que sea cómodo trabajar. Una vez conseguido resulta más ágil que en muchos editores
3. Cuando el objetivo es únicamente redactar un post, hay alternativas más sencillas como **Markdown**

## Configuración del entorno
- [Configuración del entorno en Windows](ENTORNO_WIN.md)
- Configuración del entorno en Linux
```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gynch/docbook/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
