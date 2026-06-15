*Este proyecto ha sido creado como parte del currículo de 42 por <alcristo>[Álvaro Cristóbal Olalla]*

# Libft

## DESCRIPCIÓN

Los proyectos de 42 tienen como objetivo que los estudiantes aprendan a crear código utilizando referencias y ayuda entre estudiantes. Las evaluaciones se hacen entre estudiantes sin importar el nivel entre examinador y defensor, de forma que el primero puede ayudar al segundo con su experiencia y viceversa.

Este proyecto, denominado libft, consiste en la creación de una librería de funciones llamada "libft.a", la cual será extensible y se permitirá su uso en futuros proyectos. Dicha librería tiene como objetivo entender lo que hacen las funciones más elementales. Todas las funciones poseen el prefijo "ft_".

La librería libft se puede dividir en distintas secciones:
- Funciones de libc: funciones básicas de libc, las cuales se encuenntran en el manual, creadas desde cero. Contiene las funciones isalpha, isdigit, isalnum, isascii, isprint, strlen, memset, bzero, memcpy, memmove, strlcpy, strlcat, toupper, tolower, strchr, strrchr, strncmp, memchr, memcmp, strnstr, atoi, calloc y strdup, todas ellas con el prefijo "ft_" delante para distinguirlas de sus contrapartes de libc.
- Funciones adicionales: otras funciones útiles para futuros proyectos. Principalmente trabajan con cadenas de caracteres, que permiten encontrar subcadenas (substr), unir cadenas (strjoin), recortar por ambos lados un set de caracteres (strtrim), dividir una cadena por palabras (split), convertir un entero en cadena (itoa), aplicar una función a cada carácter creando una nueva cadena (strmapi) o directamente sobre la cadena (striteri) y escribir caracteres, cadenas con o sin salto de línea y enteros sobre un descriptor de archivo (putchar, putstr, putendl y putnbr, todas ellas con el sufijo "\_fd"). Todas estas funciones también poseen el prefijo "ft_".
- Funciones de listas enlazadas: funciones que permiten trabajar con listas enlazadas. Pueden crear un nodo (lstnew), añadir uno a la cabeza (lstadd\_front) o a la cola (lstadd\_back), contar el número de nodos (lstsize), ir al último nodo de la lista (lstlast), eliminar un nodo (lstdelone) o toda la lista (lstclear) y aplicar funciones sobre la lista (lstiter) o creando una lista nueva (lstmap). De nuevo, todas las funciones tienen el prefijo "ft_".

## INSTRUCCIONES

Para crear la librería simplemente se tiene que escribir en el terminal el comando make junto con la regla all, siendo ésta opcional:

```bash
make all
```

Para eliminar los archivos temporales se utiliza la regla clean. Para eliminar también la librería simplemente hay que ejecutar la regla fclean. Finalmente, para hacer todo lo descrito en este párrafo y volver a crear la librería hay que ejeutar make con la regla re.

Para utilizar la librería en un archivo .c únicamente hay que añadirle la librería:

```bash
[compilador] [-flags] libft.a [archivos.c]
```

## RECURSOS

Se tomaron como referencia algunas funciones que hice durante la piscina de 42, así como otras, principalmente el Makefile, de la Piscine Reloaded.

Debido a mi falta de entendimiento sobre la gestión de memoria con las funciones memcpy y memmove, la página web de Ana Martínez Aguilar (https://anamartinezaguilar.medium.com/funciones-para-copiar-vectores-en-c-memcpy-y-memmove-9ce124778801) me ayudó a comprender ambas funciones. No implementé el código hasta entender el correcto  funcionamiento de dichas funciones.

Se utilizó el programa "Francinette" (https://github.com/xicodomingues/francinette) para la comprobación del correcto funcionamiento de todas las funciones, así como para la gestión de fugas de memoria. También se discutió el código con otros compañeros, que ayudaron a encontrar errores.

No se ha utilizado inteligencia artificial para la elaboración de ninguna de las funciones de este proyecto, así como para el entendimiento del código y la corrección de errores..
