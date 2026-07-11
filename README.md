# UML-Java — estudio de UML Distilled + POO en Java

Claude Code es mi profesor. Yo le paso pantallazos del libro, él me los
explica en español, mantiene la guía (GUIA-UML.md) y crea ejercicios
(EJERCICIOS.md). Yo escribo todo el código Java a mano.

## Los dos lugares donde se escriben cosas
- [TERMINAL] = la consola de siempre (fish)
- [CLAUDE]   = dentro del programa, después de escribir `claude`
Cada paso dice dónde va. Los MENSAJES están al final del archivo.

## Carpetas
- paginas/         → acá dejo la tanda actual (3-5 pantallazos por vez)
- paginas/leidas/  → Claude archiva acá los ya explicados (lo hace él)
- ejercicios/      → mi código Java, una carpeta por ejercicio
- diagramas/       → mis diagramas .puml
- GUIA-UML.md      → la guía (la escribe Claude)
- EJERCICIOS.md    → los ejercicios (los escribe Claude)

============================================================
PRIMERA VEZ EN LA VIDA (sesión uml-s01)
============================================================
1.  [TERMINAL]  cd ~/Proyectos/UML-Java
2.  [TERMINAL]  mkdir -p paginas/leidas
3.  [TERMINAL]  pasá la primera tanda (3-5 pantallazos) a paginas/
4.  [TERMINAL]  claude
5.  [CLAUDE]    /rename uml-s01
6.  [CLAUDE]    /mcp        → engram tiene que decir "connected"
7.  [CLAUDE]    pegá el MENSAJE 1
8.  [CLAUDE]    cuando responda "listo", pegá el MENSAJE 3
                (la primera vez pide permiso para mover imágenes → aceptá)
9.  ¿Querés seguir estudiando? → pasá la siguiente tanda de 3-5 a
    paginas/ (desde el explorador, sin cerrar Claude) y pegá el
    MENSAJE 3 otra vez. Repetí las veces que quieras.
10. [CLAUDE]    al terminar el día, pegá el MENSAJE 5
11. [CLAUDE]    salí con Ctrl+D
12. [TERMINAL]  engram search "tema de hoy" --project UML-Java
                → si aparece algo, se guardó bien. Fin del día.

============================================================
CADA DÍA DE ESTUDIO (uml-s02, s03, ...)
============================================================
1.  [TERMINAL]  pasá la primera tanda (3-5 pantallazos) a paginas/
2.  [TERMINAL]  cd ~/Proyectos/UML-Java
3.  [TERMINAL]  claude
4.  [CLAUDE]    /rename uml-sNN     ← el número que sigue (s02, s03...)
5.  [CLAUDE]    /mcp                → engram "connected"
6.  [CLAUDE]    pegá el MENSAJE 2   → te dice dónde quedamos y qué toca
7.  [CLAUDE]    si hay ejercicios pendientes y ya hiciste alguno:
                pegá el MENSAJE 4 ANTES de pasar a páginas nuevas
8.  [CLAUDE]    pegá el MENSAJE 3   → explica la tanda y la archiva solo
9.  ¿Querés seguir? → siguiente tanda de 3-5 a paginas/ y volvé al
    paso 8. Cuántas veces lo repitas lo decidís vos cada día: puede
    ser una tanda o pueden ser muchas. No hay número fijo.
10. [CLAUDE]    al terminar el día, pegá el MENSAJE 5
11. [CLAUDE]    Ctrl+D
12. [TERMINAL]  engram search "tema de hoy" --project UML-Java
13. [TERMINAL]  (opcional) git add . && git commit -m "sesión sNN"

============================================================
SI SE CERRÓ LA TERMINAL SIN QUERER (mismo día)
============================================================
[TERMINAL]  claude --resume uml-sNN
(o `claude --resume` solo, y elegís de la lista)
OJO: esto es SOLO para retomar el mismo día. Día nuevo = sesión nueva.

============================================================
REGLAS DE ORO
============================================================
1. Normalmente una sesión por día. El número solo avanza: si un día
   abrís dos sesiones, no pasa nada.
2. Cada tanda: 3-5 imágenes MÁXIMO. La cantidad de tandas por día es
   libre — la decido yo según el día.
3. NUNCA salir sin pegar el MENSAJE 5: es lo que guarda todo.
4. En días largos: si Claude empieza a olvidar cosas dichas antes o
   se pone lento, terminá la tanda en curso, pegá el MENSAJE 5, Ctrl+D,
   y seguí en una sesión nueva (número siguiente, mismo día).

============================================================
MENSAJES PARA COPIAR Y PEGAR
============================================================

--- MENSAJE 1 — inicial (solo en uml-s01) ---

```
Este es un proyecto de estudio y vos sos mi profesor particular.

QUIÉN SOY
- Novato total en POO/Java y novato total en UML. No asumas nada.
- Objetivo: escribir código bien estructurado y conseguir mi primer empleo
  como desarrollador.
- El libro es "UML Distilled" (Martin Fowler, 3ra ed.) en inglés; yo leo
  mejor en español.

FLUJO POR CADA TANDA DE PÁGINAS (máx. 3-5 imágenes que dejo en paginas/)
1. TRADUCCIÓN EXPLICADA: contame en español TODO lo que dicen esas páginas,
   con tus palabras, reordenado para un novato, sin saltarte ningún
   concepto. No es traducción literal del libro: es una explicación
   completa con tus propios ejemplos. Los términos técnicos clave dejalos
   también en inglés entre paréntesis (los necesito para entrevistas).
2. UML <-> JAVA: conectá cada concepto con Java mostrando el ejemplo mínimo
   de código EN EL CHAT, con comentario // en cada línea relevante. Si el
   tema necesita una base de Java que no vimos (interfaces, herencia,
   colecciones...), frená y explicá esa base primero, con analogías.
3. COMPRENSIÓN: antes de cerrar, haceme 1-2 preguntas cortas para verificar
   que entendí. Si respondo mal, explicalo de otra forma.
4. GUÍA: actualizá GUIA-UML.md agregando la sesión con el formato del
   archivo, y sumá los términos nuevos a la tabla de vocabulario.
5. EJERCICIOS: cuando el tema lo amerite, agregá ejercicios a EJERCICIOS.md
   con su formato (número, tema, tipo, enunciado claro, dónde entrego, y
   "Si te trabás: revisá la Sesión #Y"). Los hago de a uno por día.
6. ENGRAM: guardá en Engram (project "UML-Java") los conceptos clave, las
   decisiones y en qué página quedamos.

NOTA: en un mismo día puedo pasarte varias tandas seguidas (yo decido
cuántas). Cada tanda repite este flujo completo desde el paso 1.

REGLAS FIJAS
- Yo escribo TODO el código Java a mano en ejercicios/. Vos no creás ni
  editás archivos .java: mostrás ejemplos en el chat y corregís lo mío.
- SÍ podés editar directamente GUIA-UML.md y EJERCICIOS.md.
- No ejecutes bash salvo que te lo pida explícitamente.
- Puedo frenarte en cualquier momento con una duda: resolvela con calma y
  detalle antes de seguir.
- Si hay algo importante que el libro no dice pero debería saber (buenas
  prácticas, cómo se usa en el trabajo real), decímelo y anotalo en la
  guía como "NOTA DEL PROFE".

ARRANQUE DE HOY
1. Leé CLAUDE.md, GUIA-UML.md y EJERCICIOS.md.
2. Buscá en Engram (project "UML-Java") si hay progreso previo.
3. Confirmame en una línea qué encontraste y decime "listo para la primera
   tanda".
```

--- MENSAJE 2 — arranque del día (s02 en adelante) ---

```
Nueva sesión de estudio. Leé CLAUDE.md, GUIA-UML.md y EJERCICIOS.md, buscá
en Engram (project "UML-Java") dónde quedamos, y decime: (1) qué vimos la
última vez en una línea, (2) qué ejercicios tengo pendientes, (3) qué toca
hoy. Después decido si corregimos un ejercicio o te paso la siguiente tanda.
```

--- MENSAJE 3 — tanda de páginas (repetible: una vez por cada tanda) ---

```
Tanda nueva: leé todas las imágenes que hay en la raíz de paginas/
(sin entrar a paginas/leidas/), en orden de nombre, y arrancá el flujo.
Cuando termines de explicarme esta tanda, antes de seguir con cualquier
otra cosa, mové esas mismas imágenes a paginas/leidas/ para que la raíz
quede vacía.
```

--- MENSAJE 4 — corregir un ejercicio ---

```
Hice el ejercicio #NN, está en ejercicios/ejNN-nombre/. Revisalo línea por
línea: qué está bien, qué está mal y POR QUÉ, y actualizá su estado y tu
corrección en EJERCICIOS.md.
```

--- MENSAJE 5 — cierre (SIEMPRE antes de salir) ---

```
Cerramos acá:
1. Verificá que GUIA-UML.md y EJERCICIOS.md quedaron actualizados con
   todo lo de hoy.
2. Guardá en Engram (project "UML-Java") el resumen y en qué página
   quedamos.
3. Dame el resumen final de la sesión.
```
