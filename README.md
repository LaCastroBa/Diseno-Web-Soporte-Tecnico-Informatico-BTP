# Diseño Web · Taller en tres niveles

Material de Diseño Web para 1.er año del BTP Soporte Técnico Informático (DGETP-UTU).

Cada uno de los 33 contenidos del programa tiene **tres niveles**: básico, intermedio y avanzado. Todo el grupo trabaja el mismo tema en la misma clase, y cada estudiante elige el escalón que le corresponde.

## Qué hay en este repositorio

| Archivo | Para qué sirve |
|---|---|
| `index.html` | **Taller de Diseño Web.** Los 33 contenidos (unidades 1 a 5). Cada tema tiene una analogía y tres pestañas (Básico, Intermedio, Avanzado), cada una con su explicación y su ejercicio: zona de práctica, botón **Abrir en CodePen** y botón **Descargar para VS Code**. Incluye el programa con acceso directo a cada nivel, la rúbrica del proyecto, la lista de entregas y el glosario. |
| `guia-estudiante.html` | **Diseño Web desde cero.** Guía paso a paso para estudiantes de 14 años sin conocimientos previos: 4 pasos de introducción y uno por cada tema, con analogía, explicación sencilla, cómo se hace, código para copiar y error común. Cada paso enlaza a los tres niveles del taller. |
| `.nojekyll` | Le indica a GitHub Pages que publique los archivos tal cual. |

Las dos páginas son archivos HTML únicos: no hay que instalar nada.

## Publicar en GitHub Pages

1. En GitHub, botón **New** → nombre del repositorio (por ejemplo `diseno-web-btp`) → **Public** → **Create repository**.
2. **uploading an existing file** → arrastrá `index.html`, `guia-estudiante.html`, `README.md` y `.nojekyll` → **Commit changes**.
   - Si `.nojekyll` no aparece al arrastrar, creálo con **Add file → Create new file**, nombre `.nojekyll`, vacío.
3. **Settings → Pages** → *Source*: **Deploy from a branch** → rama **main**, carpeta **/ (root)** → **Save**.
4. A los 1 o 2 minutos el taller queda en `https://TU-USUARIO.github.io/diseno-web-btp/` y la guía en `.../guia-estudiante.html`.

Si ya tenías publicada la versión anterior, subí estos archivos al mismo repositorio con **Add file → Upload files**: reemplazan a los viejos y el link no cambia.

## Cómo se usa en clase

- **Mi nivel** (arriba a la derecha, B · I · A): cada estudiante elige su nivel y los temas se abren en ese nivel. Puede cambiar de pestaña cuando quiera.
- **Ver los tres juntos**: en cada tema, una pestaña muestra las explicaciones y consignas de los tres niveles una debajo de otra. Sirve para planificar o proyectar en clase.
- **Programa**: tabla con los 33 contenidos y un acceso directo a cada nivel.
- Los puntitos de colores en el índice muestran qué niveles terminó cada estudiante.

Una forma de organizar la clase: explicación común de 10 minutos con la analogía y el básico, y después cada uno trabaja en su nivel. Quien termina el básico pasa al intermedio.

## Cómo trabajan los estudiantes

- **Zona de práctica:** editan HTML, CSS y JS (pestañas) y ven el resultado con su consola. **Ctrl + Enter** ejecuta. El código queda guardado en ese navegador.
- **CodePen:** *Abrir en CodePen* crea un Pen con el código. Lo guardan con *Save* y pegan el link en el ejercicio.
- **Visual Studio Code:** *Descargar para VS Code* baja un `index.html` completo para abrir con Live Server.
- **Entregas:** al marcar *Lo terminé*, el ejercicio aparece en **Mis entregas**. Ahí completan nombre y grupo y copian el resumen para pegarlo en CREA (o lo descargan como .txt).

> El progreso se guarda en el navegador de cada estudiante (localStorage). Si cambian de computadora o borran los datos del navegador, se pierde: lo que vale como entrega es el link de CodePen o GitHub.

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
- Si un ejercicio no tiene `h`, `s` ni `j`, es de respuesta escrita (sin zona de práctica).
- Si un código incluye la etiqueta de cierre de script, escribila como `<\/script>`.
- La guía para estudiantes está en `guia-estudiante.html`, en `var GUIA = {`.

La rúbrica está en `var RUBRICA` y el glosario en `var GLOSARIO`.

## Mapa del programa

| Unidad | Contenidos |
|---|---|
| 1 · Fundamentos de diseño web | 1.1 a 1.4 |
| 2 · Fundamentos de HTML y CSS | 2.1 a 2.8 |
| 3 · Diseño web interactivo | 3.1 a 3.8 |
| 4 · Diseño web avanzado | 4.1 a 4.8 |
| 5 · Proyecto web | 5.1 a 5.5 |

Todos los contenidos tienen nivel básico, intermedio y avanzado.

Fuente: [Programa de Diseño Web, BTP Soporte Técnico Informático (DGETP-UTU)](https://planeamientoeducativo.utu.edu.uy/sites/planeamientoeducativo.utu.edu.uy/files/2025-04/Dise%C3%B1o_Web_T7I_TP.pdf).
