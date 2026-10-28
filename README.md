# Diseño Web - Recurso en tres niveles

Material de Diseño Web para 1.er año del BTP Soporte Técnico Informático (DGETP-UTU).

Cada uno de los contenidos del programa tiene **tres niveles**: básico, intermedio y avanzado. Todo el grupo trabaja el mismo tema en la misma clase, y cada estudiante elige el nivel que le corresponde.

## Qué hay en este repositorio

| Archivo | Para qué sirve |
|---|---|
| `index.html` | **Diseño Web.** Los contenidos (unidades 1 a 5). Cada tema tiene una analogía y tres pestañas (Básico, Intermedio, Avanzado), cada una con su explicación y su ejercicio. Básico e intermedio se hacen en **CodePen** y avanzado en **Visual Studio Code**. Incluye el programa con acceso directo a cada nivel, la rúbrica del proyecto, la lista de entregas y el glosario. |
| `guia-estudiante.html` | **Diseño Web desde cero.** Guía paso a paso para estudiantes de 14 años sin conocimientos previos: pasos de introducción y uno por cada tema, con analogía, explicación sencilla, cómo se hace, código para copiar y error común. Cada paso enlaza a los tres niveles del curso. |
| `primeros-pasos.html` | **Mis primeros pasos.** Recorrido corto para estudiantes a los que les cuesta empezar: eligen un tema (videojuego, celular, app o consola) y hacen su primera página en 7 pasos cortos, de a uno por vez. Funciona en el celular, revisa cada paso y dice qué arreglar, guarda el avance y al final se entrega por el mismo formulario del curso. |
| `.nojekyll` | Le indica a GitHub Pages que publique los archivos tal cual. |

Todas las páginas son archivos HTML únicos: no hay que instalar nada.

## Cómo se usa en clase

- **Mi nivel** (arriba a la derecha, B · I · A): cada estudiante elige su nivel y los temas se abren en ese nivel. Puede cambiar de pestaña cuando quiera.
- **Ver los tres juntos**: en cada tema, una pestaña muestra las explicaciones y consignas de los tres niveles una debajo de otra. Sirve para planificar o proyectar en clase.
- **Programa**: tabla con los contenidos y un acceso directo a cada nivel.
- Los puntos de colores en el índice muestran qué niveles terminó cada estudiante.

Una forma de organizar la clase: explicación común de 10 minutos con la analogía y el básico, y después cada uno trabaja en su nivel. Quien termina el básico puede pasar al intermedio.

## Cómo trabajan los estudiantes

| Nivel | Herramienta | Qué entregan |
|---|---|---|
| Básico | CodePen | El enlace del Pen guardado (o el código pegado, si no pudieron guardar) |
| Intermedio | CodePen | El enlace del Pen guardado (o el código pegado, si no pudieron guardar) |
| Avanzado | Visual Studio Code + Live Server | Sus archivos: `index.html` y, si los tienen, `.css` y `.js` |

- **CodePen:** *Abrir en CodePen* crea un Pen con el código para empezar. Lo guardan con *Save* (necesitan cuenta gratis) y pegan el link en el ejercicio. El curso avisa si el link es de un Pen sin guardar.
- **Visual Studio Code:** *Descargar para VS Code* baja un `index.html` para abrir con Live Server. Al terminar eligen sus archivos en el curso y pueden ver una vista previa antes de entregar.
- **Ejercicios de respuesta escrita:** se responden en el mismo curso, en cualquier nivel.
- **Entregas:** con el botón **Entregar** (ver más abajo). En **Mis entregas** ven qué entregaron y qué les falta.

> El progreso se guarda en el navegador de cada estudiante (localStorage). Si cambian de computadora o borran los datos del navegador, se pierde la marca de "terminado", pero las entregas ya enviadas quedan en tu formulario.

## Entregas por Formulario de Google (sin cuentas)

Debajo de cada ejercicio hay un botón **Entregar**. Abre el Formulario de Google en otra pestaña con el nombre, el tema, el nivel, el ejercicio, el enlace, la respuesta escrita y el código (HTML, CSS y JS) ya escritos: el estudiante solo toca **Enviar**. No necesita ninguna cuenta. Todo te llega a la planilla del formulario, una fila por entrega. Si el código es muy largo para entrar en el link, el curso lo copia y el estudiante lo pega en la pregunta HTML.

## Cómo editar o agregar ejercicios

Abrí `index.html` en VS Code y buscá `tema({ id: '1.1'`. Cada tema tiene este formato:

```js
tema({ id: '2.1', u: '2', t: 'Elementos, etiquetas y atributos HTML',
  a: `Analogía del tema`,
  b: { x: `Explicación del nivel básico`,
       e: { t: 'Título del ejercicio', c: `Consigna`,
            k: ['Criterio 1', 'Criterio 2'], p: `Pista`,
            h: `HTML inicial`, s: `CSS inicial`, j: `JS inicial` } },
  i: { ... nivel intermedio ... },
  v: { ... nivel avanzado ... }
});
```

- En los textos: `**negrita**`, `~código~`, líneas que empiezan con `- ` son listas y con `1. ` listas numeradas.
- Si un ejercicio no tiene `h`, `s` ni `j`, es de respuesta escrita. Si tiene código, en básico e intermedio se abre en CodePen y en avanzado se descarga para VS Code.
- Si un código incluye la etiqueta de cierre de script, escribila como `<\/script>`.
- La guía para estudiantes está en `guia-estudiante.html`, en `var GUIA = {`.
- La rúbrica está en `var RUBRICA` y el glosario en `var GLOSARIO`.

## Mapa del programa

| Unidad | Contenidos |
|---|---|
| 1 · Fundamentos de diseño web | 1.1 a 1.4 |
| 2 · Fundamentos de HTML y CSS | 2.1 a 2.8 |
| 3 · Diseño web interactivo | 3.1 a 3.8 |
| 4 · Diseño web avanzado | 4.1 a 4.8 |
| 5 · Proyecto web | 5.1 a 5.5 |

Todos los contenidos tienen nivel básico, intermedio y avanzado.

## Sobre este recurso

Recurso Educativo Abierto creado para estudiantes de 1.er año del BTP Soporte Técnico Informático (DGETP-UTU), de la unidad curricular Diseño Web.

Este recurso ha sido creado reconociendo la diversidad y los diferentes niveles de aprendizaje presentes en el aula. Aplicando los principios del Diseño Universal para el Aprendizaje (DUA), los contenidos y actividades se estructuran en tres niveles de complejidad progresiva. Esta arquitectura multinivel garantiza múltiples formas de acción, expresión e implicación, permitiendo que cada estudiante acceda al objetivo de aprendizaje a través de un andamiaje personalizado y adaptado a su competencia actual, eliminando barreras de forma integrada.

Material elaborado a partir de:

Fuente: [Programa de Diseño Web, BTP Soporte Técnico Informático (DGETP-UTU)](https://planeamientoeducativo.utu.edu.uy/sites/planeamientoeducativo.utu.edu.uy/files/2025-04/Dise%C3%B1o_Web_T7I_TP.pdf).

**Autoría:** Ed. Tec. Laura Castro. El diseño didáctico y la organización son de elaboración propia y se comparten bajo licencia [Creative Commons Atribución-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es).
