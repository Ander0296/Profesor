GUÍA-ARCHIVO: UML DISTILLED — sesiones históricas (#01 a #09)

Archivo de consulta OCASIONAL — NO se lee al inicio de sesión.
Contiene las sesiones completas en el formato largo original, movidas
acá el 2026-07-24 para mantener liviana la guía activa (GUIA-UML.md).
Se consulta SOLO para RE-ESTUDIO (repaso mal dos veces seguidas) o
cuando el usuario pide releer una sesión vieja puntual. Las sesiones
#10 en adelante viven en GUIA-UML.md en formato corto.

============================================================

============================================================
SESIÓN #01 — 2026-07-11 — Prólogo 3ra edición (Cris Kobryn) (Ubicación 332-358, 6-7%)
============================================================

IDEAS CLAVE
- Ley de la parsimonia: los mejores diseños de la historia (pirámides,
  UNIX, Smalltalk) siguen "menos es más" / Occam's Razor.
- Kobryn presidió la estandarización de UML 2.0 y admite que el proceso
  de comité agregó complejidad gratuita ("design by committee").
  Por eso valora que Fowler haya distilado el 20% de UML que resuelve
  el 80% del trabajo real (principio de Pareto).
- UML tiene dos usos bien distintos: "pararrayos de creatividad"
  (boceto informal) vs. "láser de precisión" (plano tan exacto que un
  tercero podría construir el sistema con eso solo). Esta segunda es
  la "prueba ácida" de un lenguaje de planos genuino.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía no aplica — contenido puramente introductorio, sin notación
  UML mostrada aún.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- El 80/20 (Pareto) no es solo filosofía de diagramas: es la regla de
  oro de TODO el código. Sobre-diseñar (agregar interfaces y patrones
  que nadie pidió) es un error típico de junior. Saber cuándo parar es
  señal de senior.

DUDAS QUE SURGIERON (y su respuesta corta)
- Diferencia entre "pararrayos de creatividad" (comunicación informal)
  y "láser de precisión" (plano suficientemente completo para construir
  sin ambigüedad, no solo para que dos personas se entiendan).

EJERCICIOS CREADOS: ninguno (tema introductorio)
PRÓXIMO PASO: Foreword a la 1ra edición + Preface

============================================================
SESIÓN #02 — 2026-07-11 — Foreword 1ra edición + Preface + inicio "Why Bother with the UML?" (Ubicación 362-406, 8-9%)
============================================================

IDEAS CLAVE
- "The Three Amigos" (Booch, Jacobson, Rumbaugh) crearon UML unificando
  tres métodos de modelado OO que competían en los 90. Crear UML fue
  en sí un proceso iterativo e incremental.
- Fowler explica el propósito del libro: deliberadamente breve, busca
  la fracción de UML más útil (mismo concepto 80/20 de la Sesión #01).
  Es un libro CON OPINIÓN (no pretende ser neutral).
- El libro NO enseña OO desde cero (para eso recomienda a Larman) —
  ese hueco lo cubrimos nosotros en el chat.
- Los ejemplos de código del libro son en Java y C#.
- Valor principal de un diagrama: comunicación y entendimiento en
  equipo, no reemplazar el código. Fowler es escéptico de que lo
  gráfico algún día reemplace al texto/código.
- UML se volvió importante por su adopción masiva y estandarización
  dentro (y fuera) del mundo OO.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía no aplica — sigue siendo introducción. Dato a retener: los
  próximos ejemplos de código del libro (y los nuestros) van a ser en
  Java.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Frase para grabar: "UML es un asistente, no un reemplazo del código."
  Se usa para pensar y comunicar antes o en paralelo al código, nunca
  en vez de escribirlo.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — ambas respuestas de verificación fueron correctas.

EJERCICIOS CREADOS: ninguno (tema introductorio)
PRÓXIMO PASO: seguir "Why Bother with the UML?" y entrar a los primeros
conceptos concretos de UML.

============================================================
SESIÓN #03 — 2026-07-11 — Acknowledgments (Ubicación 449-485, 11-12%)
============================================================

IDEAS CLAVE
- Sección de agradecimientos de Fowler, sin contenido técnico nuevo.
- Craig Larman reaparece como revisor (mismo autor recomendado antes
  para aprender OO desde cero).

UML <-> JAVA (cómo se ve cada concepto en código)
- No aplica.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Ninguna esta vez.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — tanda sin contenido conceptual, no se hizo verificación.

EJERCICIOS CREADOS: ninguno
PRÓXIMO PASO: arranca el cuerpo del libro — primeros conceptos
concretos de UML.

============================================================
SESIÓN #04 — 2026-07-11 — Cap. 1 Introducción: "What Is the UML?" + arranca "Ways of Using the UML" (Ubicación 487-513, 12-14%)
============================================================

IDEAS CLAVE
- UML = familia de notaciones gráficas respaldadas por un único
  meta-modelo, para describir/diseñar sistemas OO. Existe porque el
  código no tiene nivel de abstracción suficiente para discutir diseño.
- UML lo controla el OMG (Object Management Group), conocido también
  por CORBA. Nació unificando varios lenguajes gráficos OO de fines
  de los 80/principios de los 90.
- Fowler y Steve Mellor identificaron 3 formas de usar UML: sketch,
  blueprint y programming language (el 3ro todavía no se vio).
- Sketch (boceto) = selectivo/informal, mostrás solo lo importante.
  Blueprint (plano) = completo/detallado, el programador solo codifica
  lo que el diseñador ya decidió.
- Forward engineering (diagrama antes del código) y reverse engineering
  (diagrama a partir del código ya existente) son un EJE INDEPENDIENTE:
  tanto sketch como blueprint pueden hacerse en cualquiera de las dos
  direcciones.
- La mayoría de los diagramas de este libro (y de la mayoría de los
  libros) son bocetos, no planos completos.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía sin notación concreta de diagramas. Se conectó con el propio
  flujo de trabajo del proyecto: diseñar en el chat antes de escribir
  código en ejercicios/ = forward engineering + sketch; diagramar en
  diagramas/*.puml a partir de código ya escrito = reverse engineering
  + sketch.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Sketch vs. blueprint es probablemente el concepto más citado del
  libro y sale en entrevistas técnicas. En la industria real casi
  nadie hace "blueprint" completo — se usa mucho más como boceto
  rápido de pizarra para alinear al equipo antes de codear.

DUDAS QUE SURGIERON (y su respuesta corta)
- Confusión inicial: pensar que "sketch" se define por ser hecho A
  PARTIR del código (reverse). Corrección: sketch/blueprint (qué tan
  completo) y forward/reverse (en qué dirección) son dos ejes
  independientes — ambos modos admiten las dos direcciones.

EJERCICIOS CREADOS: ninguno todavía
PRÓXIMO PASO: tercer modo "UML as programming language" y seguir
Capítulo 1.

============================================================
SESIÓN #05 — 2026-07-11 — Cierre "Ways of Using the UML" + MDA + Executable UML (Ubicación 525-553, 14-15%)
============================================================

IDEAS CLAVE
- Blueprint puede ser parcial (solo interfaces de subsistemas) o total.
  En reverse engineering, un blueprint muestra el detalle de una clase
  en forma gráfica.
- Herramientas CASE (término hoy evitado por sobreventa de los 90):
  forward-engineering tools, reverse-engineering tools, round-trip
  tools (hacen ambas), y "tripless tools" (el código ES el repositorio,
  el diagrama es solo una vista).
- Frase resumen: "los bocetos son exploratorios, los planos son
  definitivos."
- 3er modo: UML as programming language — el diagrama se compila
  directo a código ejecutable; diagrama y código son la misma cosa,
  por eso forward/reverse engineering dejan de tener sentido ahí.
- MDA (Model Driven Architecture, estándar del OMG): PIM (modelo
  independiente de plataforma) -> PSM (modelo específico de una
  plataforma) -> código. Si todo el proceso es automático = UML as
  programming language; si algún paso es manual = blueprint.
- Executable UML (Mellor): salta el PSM, usa un "model compiler" +
  "archetypes" para ir directo de modelo a sistema desplegable en un
  paso automático. Usa menos construcciones que el UML completo.

UML <-> JAVA (cómo se ve cada concepto en código)
- Conexión directa con este proyecto: siempre vamos a trabajar en modo
  "UML as sketch" — nunca se compila un diagrama a Java acá, el
  usuario escribe todo el código a mano.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- MDA y Executable UML son nicho (embebidos, aeroespacial,
  telecomunicaciones) y no hace falta memorizarlos para el primer
  laburo. Lo que sí hay que tener sólido es la distinción
  sketch / blueprint / programming language.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — ambas respuestas de verificación fueron correctas al
  primer intento.

EJERCICIOS CREADOS: ninguno todavía
PRÓXIMO PASO: seguir Capítulo 1 — próximos temas de la introducción.

============================================================
SESIÓN #06 — 2026-07-15 — Detalle MDA/Executable UML + perspectivas + arranca "How We Got to the UML" (Ubicación 550-596, 15-17%)
============================================================

IDEAS CLAVE
- MDA en detalle: PIM único -> PSM por plataforma (vía herramientas de
  vendors) -> código. Si TODO el proceso es automático = UML as
  programming language; si algún paso es manual = blueprint.
- Executable UML en detalle: un Model Compiler va directo del modelo
  (equivalente al PIM) a un sistema desplegable, en un paso 100%
  automático, salteando el PSM. Se basa en archetypes: reglas que le
  dicen al compiler cómo llevar el modelo a una plataforma concreta
  (ej. comprás un compiler + archetypes J2EE y .NET).
- Fowler es escéptico de "UML as programming language" en la práctica:
  duda de madurez de herramientas y, sobre todo, de que lo gráfico sea
  más productivo que lo textual. Compara con Smalltalk (muy productivo
  pero nunca llegó a masa crítica, quedó nicho) — teme el mismo destino.
- UML 2 tiene tres formas de behavioral modeling (interaction, state,
  activity diagrams) — solo mencionadas, todavía sin detalle.
- Perspectiva de software vs. perspectiva conceptual: en la de software
  los elementos del diagrama mapean casi directo a elementos de un
  sistema real que se va a programar; en la conceptual el diagrama
  describe conceptos de un dominio, sin pensar en software. Es un
  espectro, no una regla estricta.
- "Esencia de UML": para la mayoría (usuarios de sketch) son los
  diagramas; para los creadores de UML, la esencia es el meta-modelo y
  los diagramas son solo su presentación.
- Fowler declara su sesgo: usa UML casi siempre como sketch, es
  escéptico de blueprints forward-engineered detallados (frenan el
  desarrollo) y considera que el valor de un blueprint reverse-engineered
  depende de si la herramienta es navegable o solo genera un documento
  estático ("mata árboles").
- Arranca sección nueva "How We Got to the UML" (historia) — todavía
  sin contenido, solo el título.

UML <-> JAVA (cómo se ve cada concepto en código)
- Perspectiva de software: una clase "Cuenta" en el diagrama mapea casi
  1 a 1 a una clase Java `Cuenta` con sus atributos y métodos.
- Perspectiva conceptual: el mismo nombre "Cuenta" puede aparecer en un
  diagrama solo para acordar qué significa el término en un dominio de
  negocio, sin que eso implique ninguna clase Java concreta.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- La distinción software/conceptual perspective es más relevante en el
  día a día que MDA/Executable UML: te ayuda a leer un diagrama ajeno y
  saber si te está mostrando "así va a ser el código" o "así entendemos
  el negocio". El resto de esta sesión (MDA, Executable UML, esencia
  del UML) es contexto/nicho — no hace falta memorizarlo.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — ambas respuestas de verificación fueron correctas. Se afinó
  el criterio de la primera: lo que define "perspectiva de software" no
  es que el diagrama mencione el lenguaje de programación, sino que sus
  elementos mapeen directo a elementos de un sistema real.

EJERCICIOS CREADOS: ninguno todavía (sigue siendo contenido conceptual,
sin notación de diagramas)
PRÓXIMO PASO: seguir "How We Got to the UML" (historia de UML).

============================================================
SESIÓN #07 — 2026-07-15 — Historia real de UML (Three Amigos, OMG) + notación vs. meta-modelo + Figura 1.1 (Ubicación 616-657, 18-20%)
============================================================

IDEAS CLAVE
- Historia (contexto/nicho, buen dato de entrevista): en los 80 los
  objetos salen del laboratorio al mundo real (Smalltalk se estabiliza,
  nace C++). Entre 1988-1992 aparecen los libros clave de modelado OO
  gráfico: Booch, Coad, Jacobson (Objectory/OOSE), Odell, Rumbaugh
  (OMT), Shlaer & Mellor, Wirfs-Brock (Responsibility Driven Design).
  Métodos muy parecidos en concepto pero con notaciones distintas ->
  confusión real en los equipos.
- Evento cataclísmico: Jim Rumbaugh deja GE y se une a Grady Booch en
  Rational -> "Unified Method" v0.8 (OOPSLA '95). Rational compra la
  empresa de Ivar Jacobson -> se completan "los Tres Amigos" (Booch,
  Rumbaugh, Jacobson).
- Lo que metió al OMG en el tema NO fueron los metodólogos rivales:
  fueron los FABRICANTES DE HERRAMIENTAS CASE, con miedo a que un
  estándar controlado por Rational les diera ventaja desleal. Bandera:
  "interoperabilidad entre herramientas CASE".
- 1997: Rational presenta v1.0 de la documentación UML; el OMG adopta
  la v1.1 como estándar oficial. Revisiones: 1.2 cosmética, 1.3 más
  significativa, 1.4 agrega detalle de componentes/profiles, 1.5 agrega
  action semantics.
- Fowler opina que darle TODO el crédito a los "Tres Amigos" es algo
  injusto: la notación nació en el método unificado Booch/Rumbaugh,
  pero después el trabajo real lo empujaron los comités del OMG (de
  los tres, solo Rumbaugh se mantuvo comprometido en esa etapa).
- Notación vs. meta-modelo (NÚCLEO): la notación es la parte gráfica
  (cómo se dibuja cada símbolo); el meta-modelo son las reglas de fondo
  que definen con precisión qué ES cada concepto (clase, asociación,
  multiplicidad). El meta-modelo de UML es, generalmente, un diagrama
  de clases que describe los propios conceptos de UML (UML
  describiéndose a sí mismo).
- La mayoría de lenguajes gráficos de modelado tienen poco rigor formal
  (apelan a la intuición) y eso no es un problema — lo que importa es
  que sean útiles, no que sean matemáticamente exactos como en los
  métodos formales (predicate calculus).
- Figura 1.1: fragmento del meta-modelo de UML (Feature -> Structural
  Feature / Behavioral Feature, con Behavioral Feature relacionado a
  Parameter). Es solo un preview visual — el propio Fowler dice que no
  lo va a explicar acá; la lección completa de diagramas de clases
  viene en el próximo capítulo.

UML <-> JAVA (cómo se ve cada concepto en código)
- Feature = cualquier miembro de una clase Java. Structural Feature =
  atributo (campo). Behavioral Feature = método. Parameter = cada
  parámetro del método. `{ordered}` = el ORDEN POSICIONAL de los
  parámetros en la firma importa (saludar(String, int) != saludar(int,
  String)) — no tiene que ver con el orden de ejecución de acciones
  dentro del método.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- La historia (Three Amigos, versiones 1.0-1.5) es trivia útil para
  charlas técnicas pero no hace falta memorizar fechas ni números de
  revisión. Lo que sí vale la pena tener sólido es la distinción
  notación / meta-modelo — te va a servir para entender por qué a
  veces se dibuja "un diagrama de un diagrama" (meta-modelado).

DUDAS QUE SURGIERON (y su respuesta corta)
- Confusión: pensar que un "Parameter" es una acción que ejecuta el
  método, y que `{ordered}` refiere al orden en que se ejecutan esas
  acciones. Corrección: un parámetro es un DATO de entrada que el
  método recibe, no un paso de comportamiento; `{ordered}` refiere a la
  posición de cada parámetro en la firma (relevante para cómo Java
  hace matching de argumentos por posición y tipo), no a la secuencia
  de instrucciones internas del método.

EJERCICIOS CREADOS: ninguno todavía (Figura 1.1 es solo preview, sin
notación formal de diagramas de clases enseñada aún)
PRÓXIMO PASO: seguir con la próxima tanda — el libro se encamina al
capítulo de Class Diagrams.

============================================================
SESIÓN #08 — 2026-07-15 — Cierre meta-modelo + "UML Diagrams": los 13 tipos oficiales (Ubicación 669-685, 20-21%)
============================================================

IDEAS CLAVE
- Cuánto importa el meta-modelo depende del modo de uso: casi nada para
  sketchers, más para blueprinters, vital para quien usa UML as
  programming language (define su sintaxis abstracta). A la gente que
  desarrolla el propio estándar UML le importa sobre todo el
  meta-modelo, la notación queda en segundo plano para ellos. Fowler
  aclara que este libro NO es riguroso a propósito (apela a intuición,
  coherente con su sesgo hacia sketch).
- Arranca la sección "UML Diagrams": UML 2 define 13 tipos de diagrama
  oficiales (Tabla 1.1), clasificados en dos familias (Figura 1.2):
  Structure Diagram (Class, Composite Structure, Object, Component,
  Deployment, Package) y Behavior Diagram (Activity, Use Case, State
  Machine, e Interaction Diagram -> Sequence, Communication,
  Interaction Overview, Timing).
- MAPA DE RUTA DEL LIBRO (dato clave): Class Diagram es el ÚNICO tipo
  que ocupa DOS capítulos (3 y 5) -> es el núcleo absoluto del libro y
  del 80/20. Otros núcleos: Sequence (cap. 4), Object (cap. 6), Package
  (cap. 7), Use Case (cap. 9), State Machine (cap. 10). Más nicho:
  Deployment (cap. 8), Activity (cap. 11), Communication (cap. 12),
  Composite Structure (cap. 13), Component (cap. 14), Interaction
  Overview (cap. 16), Timing (cap. 17).
- Los propios autores de UML no ven los diagramas como lo central de
  UML (para ellos es el meta-modelo) -> por eso los tipos de diagrama
  no son rígidos: se pueden usar legalmente elementos de un tipo en
  otro: el estándar solo sugiere, no obliga.

UML <-> JAVA (cómo se ve cada concepto en código)
- Class Diagram -> las clases/interfaces que se escriben en Java.
- Package Diagram -> mapea literal a la keyword `package` de Java:
  agrupa clases y define dependencias entre paquetes (ej. `controller`
  depende de `service`), igual que un `import` en código.
- State Machine Diagram -> ciclo de vida de un objeto (ej. Pedido:
  PENDIENTE -> ENVIADO -> ENTREGADO), típicamente un `enum` en Java.
- Sequence Diagram -> el orden de llamadas a métodos entre objetos.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Esta tabla es el mapa de ruta más útil de toda la guía hasta ahora:
  ya sabemos que Class Diagram (cap. 3 y 5) es donde hay que invertir
  más tiempo y profundidad, coherente con la regla de Pareto del
  proyecto. El resto se puede ver con menos detalle salvo que el
  trabajo futuro lo pida específicamente.

DUDAS QUE SURGIERON (y su respuesta corta)
- El usuario relacionó "Package Diagram" con "programación orientada a
  objetos" en general. Se aclaró que la conexión es más puntual y
  literal: Package Diagram mapea directo a la keyword `package` de
  Java (organización de clases en paquetes + dependencias entre
  paquetes), no a POO como concepto amplio.

EJERCICIOS CREADOS: ninguno todavía (sigue siendo contenido de mapa/
organización, sin notación de diagramas enseñada en profundidad aún)
PRÓXIMO PASO: seguir con la próxima tanda — cada vez más cerca del
Capítulo 3, Class Diagrams (núcleo del libro).

============================================================
SESIÓN #09 — 2026-07-15 — Legal UML + supresión + significado de UML + "UML no alcanza" (Ubicación 686-730, 21-23%)
============================================================

IDEAS CLAVE
- Reglas prescriptivas (un organismo oficial dicta qué es legal, ej.
  lenguajes de programación) vs. reglas descriptivas (se entienden por
  cómo la gente usa el lenguaje en la práctica, ej. un idioma natural).
  UML se comporta más como reglas descriptivas: el estándar es la
  mayor influencia pero no la única, también cuentan las convenciones
  de la industria y de cada equipo.
- Terminología que Fowler usa en el resto del libro: "conventional use"
  (uso muy difundido pero fuera del estándar) vs. "standard/normative"
  (conforme al estándar; non-normative = no estrictamente legal en UML).
- Principio de SUPRESIÓN (NÚCLEO): un diagrama puede ocultar info a
  propósito (general o específicamente). Por eso nunca se puede inferir
  nada de una AUSENCIA en un diagrama — ni siquiera si el meta-modelo
  tiene un valor default, porque no hay forma de distinguir "es el
  default" de "fue suprimido" solo mirando el diagrama.
- Es más importante un buen diseño que UML "legal" si sos sketcher o
  blueprinter (excepción: UML as programming language, ahí sí tiene
  que ser legal o el programa no corre).
- "El significado de UML": el estándar no define formalmente cómo UML
  mapea a un lenguaje de programación concreto. No se puede saber el
  código EXACTO desde un diagrama, pero sí una idea aproximada — y en
  la práctica alcanza. Cada equipo arma sus propias convenciones de
  mapeo diagrama->código.
- "UML no alcanza" (NÚCLEO): la lista de tipos de diagrama de UML no es
  exhaustiva. Si ningún diagrama UML sirve para un caso puntual, está
  bien usar o inventar un diagrama que no sea UML. Ejemplo del libro:
  Figura 1.3, un "screen flow diagram" informal (pantallas de una UI y
  cómo se navega entre ellas) — ni siquiera es parte de UML, pero
  Fowler lo usó durante años porque es útil.

UML <-> JAVA (cómo se ve cada concepto en código)
- Supresión: un diagrama de `List` puede mostrar solo `add()` y `get()`
  sin que eso signifique que la interfaz no tiene más métodos — fueron
  suprimidos para legibilidad, ausencia != inexistencia.
- Screen flow diagram: útil para planear la navegación entre pantallas
  de una app ANTES de escribir las clases Java que la implementan.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- El principio de supresión es un hábito de lectura que vas a usar
  siempre: cuando te muestren un diagrama de clases de otro equipo,
  nunca asumas que lo que no está dibujado no existe.

DUDAS QUE SURGIERON (y su respuesta corta)
- El usuario mezcló dos ideas del texto: por qué está bien usar un
  diagrama no-UML (porque la lista de diagramas UML no es exhaustiva)
  con la regla de que UML debe ser legal solo si se usa como lenguaje
  de programación (un punto distinto, de la sección anterior). Se
  aclaró que son dos razones independientes.

EJERCICIOS CREADOS: #01 (screen flow diagram informal)
PRÓXIMO PASO: seguir con la próxima tanda — cada vez más cerca del
Capítulo 3, Class Diagrams (núcleo del libro).

