# Declaración de uso de IA — Práctica 1

**Grupo:** *4* · **Integrantes:** *Carlos Chapman Peña*, *Miguel Ángel Gordillo Masero*, *María Xiaolan Ríos Díaz*, *Pablo Sola Díaz*
**Fecha:** *09/11/2026*

---

## Para qué sirve este fichero

En esta asignatura el uso de IA generativa está **permitido, con declaración**, y este fichero es
esa declaración. Es un **entregable de la Práctica 1**: si falta o está vacío, resta puntos.

Rellenarlo con sinceridad no os cuesta nada. Lo que se evalúa es vuestra comprensión, y se os
preguntará por vuestro propio cuaderno.

## Qué hay que escribir

Para la Práctica 1, indicad:

* **la herramienta o el servicio**, con su nombre: «un LLM» no es una declaración;
* **el propósito**, por ejemplo ideas, explicaciones, depuración, sugerencias de código o
  revisión de redacción;
* **los ficheros o secciones afectados**, con precisión: «Ejercicio 1(a), la parte vectorizada
  de las distancias», no «parte del código»;
* **cómo comprobasteis el resultado**. Esta es la parte que más importa: decid qué hicisteis
  para aseguraros de que era correcto.

**No hace falta adjuntar conversaciones completas ni registros de instrucciones.**

**Si no usasteis IA generativa, basta una frase que lo diga.** En ese caso, borrad la tabla y
escribid esa frase.

## Declaración

| Herramienta o servicio | Propósito | Ficheros o secciones afectados | Cómo se comprobó el resultado |
|---|---|---|---|
| *Gemini* | *Solucionar un error relacionado con las dimensiones de las matrices (broadcasting) y generalizar la clase para aceptar un número dinámico de columnas (adaptar los pesos y el cálculo de distancias de 3 a 24 columnas).* | *Ejercicio 1(b) (métodos `__init__`, `fit` y `predict`de `MiVariante`) y Ejercicio 3(a).* | *Se volvió a ejecutar la función `comprobar_estimador`del Ejercicio 1 y la rejilla del Ejercicio 3(a), verificando que se procesaba la matriz `H` sin errores de dimensión.* |
| *Gemini* | *Comprender los parámetros y el uso de la función `mostrar_paleta` para visualizar las proporciones de los clústeres.* | *Ejercicio 1 (celda en la que se visualiza la imagen recoloreada).* | *Se ejecutó la celda de visualización y se comprobó visualmente que la barra de colores se dibujaba correctamente con las proporciones esperadas.* |
| *Gemini* | *Corregir la forma de recoger los tamaños de los grupos, cambiando la asignación directa por un diccionario que organizara los valores antes de crear el DataFrame.* | *Ejercicio 4(c) y 4(e)*. | *Se ejecutó el código y se verificó que la tabla final contenía los valores correctos de los tamaños de los grupos para el K elegido en cada enlace, antes de revelar los resultados*. |
| *Gemini* | *Entender el uso de `scipy.cluster.hierarchy.linkage` y desarrollar el procedimiento para extraer y calcular el mayor salto relativo entre las alturas de fusión.* | *Ejercicio 4(a) y 4(b)*. | *Se ejecutó el bloque de código para imprimir y analizar los valores de los saltos relativos, comprobando que el umbral elegido identificaba correctamente el punto de corte óptimo en el dendrograma.* |
| *Gemini* | *Dar formato en LaTeX a los textos de las celdas Markdown para mejorar la visualización de fórmulas y variables.* | *Celdas de texto explicativo en formato Markdown de todo el cuaderno.* | *Se visualizaron las celdas Markdown para comprobar que las fórmulas, variables y expresiones matemáticas se mostraban correctamente.* |
| | | | |

## Lo que sigue siendo vuestro

El grupo es **plenamente responsable** de que todo lo entregado sea correcto: cada resultado,
el código, la interpretación, las referencias y la reproducibilidad del cuaderno. También de
**entender todo lo que entrega**.

Hay dos límites que no se negocian:

* **No se permite ninguna ayuda de IA generativa durante las preguntas individuales.**
* Si vuestra propia explicación de vuestro trabajo contradice esta declaración, el asunto es de
  **integridad académica**, no de calificación.

Las normas de integridad académica de la universidad se siguen aplicando en su totalidad.
