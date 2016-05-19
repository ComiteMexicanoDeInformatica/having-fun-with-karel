# having-fun-with-karel

Se va a crear una serie de video clases que expliquen los conceptos básicos de Karel.

La idea de este repositorio es preparar las clases con el guión de la clase y los códigos/ejemplos que se usen en ellas

El primer objetivo es crear todos los videos en el orden del temario para antes del siguiente examen nacional. Pero si notamos que un tema no fue tan claro como se pretendía replantearlo y regrabarlo para futuras clases.

El temario inicial va es el siguiente:

 1. Alcance de un objetivo específico utilizando un conjunto de operaciones de forma no ambigua y mínima:  Esto se refiere básicamente a cosas como, haz que Karel se mueva desde aquí hasta aca, haz que Karel dibuje un cuadrado, haz que Karel (o lo que sea, no tiene que ser Karel) haga algo más complejo pero que se lleva a cabo exclusivamente con (avanza, coge, deja, gira).  Esto es algo que debe ser accesible sin problema a niños con facilidad a partir de los 5 años.

 2. Uso de estructura “for”/”repetir” para minimizar código:  El siguiente paso es entender que la computadora no se “cansa” de hacer la misma operación y que una de las formas más básicas y útiles de utilizarla es haciéndola que repita muchas veces lo mismo.  Aquí comienza a haber detalles más interesantes que son:

    - Entender el concepto de inicio-fin dentro de la estructura.  Es decir, que el niño entienda que tiene que delimitar mediante un bloque el conjunto de instrucciones que va a repetir.  Este simple concepto comienza a ser inaccesible para bastante gente y con niños menores de 9 se sufre un poco para hacérselos entender, a menos claro que tengan mucha facilidad.

    - Ser capaces de anidar estructuras for, esto viene un poco de la mano del concepto de inicio-fin

    - Entender la utilidad que tiene buscar estructuras repetidas dentro de un programa para utilizarlas dentro de estrucutras for.  Por ejemplo entender que si quieres hacer una cruz puedes buscar una estructura y repetirla 4 veces.  O si quieres subir una escalera puedes buscar la estructura escalón y repetirla, etc.  Este punto requiere de facilidad y maestría, es algo que no se puede alcanzar en su máximo nivel con niños pequeños, muchas veces ni siquiera con adultos, pero es algo que se debe buscar y fomentar.

 3. Lógica booleana: Entender que dentro de un código se pueden tomar decisiones basadas en preguntas que se responden con “Sí”/”No”.  

    - El punto esencial es entender que existe la posibilidad de hacer estas preguntas para tomar decisiones.

    - El punto plus es aprender que estas preguntas se pueden juntar utilizando los operadores “Y”, “O”  y “Negación”.

 4. Estructura “If – then” / “Si – entonces”:  Entender que utilizando las preguntas anteriores se puede alterar el flujo de ejecución del programa.  Este punto requiere que el programador ya tenga claro que existe un flujo de ejecución del programa, que aunque parezca completamente trivial, no lo es.  Muchos principiantes no lo tienen 100% claro, solo veladamente claro y esto hace que el concepto de alterar el flujo del programa no haga demasiado sentido ni vean las implicaciones de comenzar a “bifurcar” la ejecución.

    - Entender el concepto de inicio-fin dentro de la estructura.  Lo mismo que en el for, pero aquí tiene incluso una cosa distinta.  Ya que lo que englobes en el inicio-fin puede ser, o no ser ejecutado. 

 5. Estructura “if – then – else” / “si – entonces – si no”:  Paso natural de la estructura anterior.  Sin embargo es importante que se entienda que la primera estructura sirve para decidir hacer o no hacer algo.  Esta estructura  sirve para hacer que el programa avance por dos caminos distintos que después se vuelven a juntar.  Este concepto debe quedar muy claro.

 6. Estructura “while” / “mientras”:  Aprender a diferenciar de manera clara las situaciones en las que se debe utilizar if y las que se debe utilizar while.  Básicamente if sirve para preguntar por una condición en un momento específico del programa y decidir algo en base a la respuesta.  While sirve para ejecutar algo mientras una condición se cumpla, situación que puede depender de factores incluso externos al equipo de cómputo.

 7. Concepto de procedimiento: Este es un tema muy conceptual y que se tiene que revisar constantemente hasta llegar a niños grandes.  El concepto básico es entender que se puede definir un “bloque” de instrucciones que desempeñan una función.  Y que ese bloque puede utilizarse en cualquier lugar del programa.  Aquí hay dos puntos muy importantes en los que hay que tener cuidado:

    - Que la funcionalidad del procedimiento esté perfectamente definida y descrita en el nombre.  La tendencia inicial de cualquier principiante es mezclar funcionalidad dentro de las funciones, en el caso de Karel por ejemplo es hacer una función que al terminar se mueva hacia la posición necesaria para la siguiente función o que llame a la siguiente función o a sí misma.  Estas son malas prácticas que deben tratar de ser evitadas.

    - Que el programador sea capaz de discernir cual es la óptima división  en bloques.  Esto es algo casi artístico y no bien definido, se logra con años de práctica, pero un maestro debería poder dar sugerencias de las mejores formas de hacerlo a los alumnos.

 8. Variables de acceso directo:  Aprender que la computadora tiene la capacidad de memorizar valores los cuales son accesibles mediante variables literales.

 9. Variables de acceso indexado [arrays]:  Aprender que se pueden crear arreglos de variables a las que se puede acceder mediante un índice.

 10. Conjuntos de valores (sets, enums): Aprender que la computadora permite representar conjuntos de valores sobre los que se pueden hacer operaciones.

 11 .Procedimientos con parámetros (por valor y por referencia).

 12 .Procedimientos con valor de retorno.

 13 .Procedimientos recursivos.  La recursión tiene varias caras que se deben identificar de manera distinta:

    - Se puede utilizar recursión para una repetir una funcionalidad que se define a sí misma.  Por ejemplo, si se desea avanzar hasta llegar a una meta se puede definir un procedimiento que sepa dar un paso, preguntar si llegó a la meta y en caso de no hacerlo repetirse a sí mismo.  Esta recursión suele ser posible sustituirla por un while.  Sin embargo he visto que a la mayoría de la gente le parece más natural.

    - Se puede utilizar la recursión para recorrer un espacio de búsqueda (este es básicamente el contar en Karel).  En este caso el procedimiento sabe procesar un estado y avanzar en una o varias de las transiciones de ese estado.  Al llegar al objetivo buscado entonces se hace algo con el camino que se lleve en memoria o lo que se haya juntado durante la búsqueda.

    - Se puede utilizar la recursión como una pila, en este caso el procesamiento sucede a la salida de la recursión.

 14 .Procedimientos recursivos 2: Implicaciones de las pilas, scopes de variables.
