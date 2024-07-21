# Variables Inmutables (val)
 Se declaran utilizando la palabra clave val. Estas variables no pueden cambiar su valor una vez inicializadas. Son similares a las constantes en otros lenguajes de programación.
# Variables mutables (var):
 Se declaran utilizando la palabra clave var. Estas variables pueden cambiar su valor en cualquier momento durante la ejecución del programa.
 # Tipos de Datos y Seguridad contra Nulos
En Kotlin, todos los tipos de datos por defecto son no nulos, lo que significa que no pueden contener un valor nulo a menos que se especifique explícitamente con el operador de nulabilidad ?. Esto se aplica tanto a las variables como a los tipos de retorno de funciones y los parámetros de función.

- Tipos No Nulos: Cuando declaramos una variable sin el operador ?, no se permite asignarle un valor nulo
- Tipos Nulos: Para permitir que una variable pueda contener null, debes usar el operador ?

# Opcionales
En Kotlin, el concepto de "opcionales" se refiere al manejo de tipos de datos que pueden o no contener un valor nulo. Esta característica está integrada en el sistema de tipos del lenguaje, que busca evitar los errores comunes asociados con los valores nulos (NullPointerExceptions) en otros lenguajes de programación. El sistema de tipos de Kotlin distingue entre tipos anulables y no anulables, lo que permite comprobaciones de seguridad nulas integradas y proporciona una sintaxis concisa para manejar valores anulables.

# Manejo de nulos

En Kotlin los objetos por defecto no aceptan valores nulos, para que le podamos asignar un null tendremos que indicar que ese objeto realmente puede ser null. De esta forma vamos a poder garantizar que no se no producirá un NullPointerException en tiempo de ejecución sin necesidad de llenar todo el código de comprobaciones if (a != null) o if (b == null) cuando las variables no deban ser null en ningún caso, pero también nos da una vía de escape para que podamos tener los queridos NullPointerException.
- Operador Seguro (Safe Call Operator - ?.): Permite acceder a propiedades o llamar métodos de un objeto solo si el objeto no es nulo. Si el objeto es nulo, la expresión completa se evalúa como nula.
- Operador de elvis (?:): Proporciona un valor predeterminado si una expresión es nula.
- Operador de No Nulo (!!): Permite forzar una llamada cuando se está seguro de que el valor no es nulo. Sin embargo, su uso debe ser cuidadoso ya que puede provocar una excepción NullPointerException.

# Comentarios 
Los comentarios en Kotlin se pueden definir como una opción implementada en el sistema con el fin de dar explicación al código de Kotlin, al tiempo que permite hacerlo más legible.

Tipos de comentarios en Kotlin

- Comentarios de una sola línea: también conocidos como comentarios de final de línea. Se refieren a aquellos que inician con dos barras diagonales y finalizan con el final de la línea, razón por la que el compilador del sistema ignora el texto que se escriba entre las dos barras y el final de la línea.
- Comentarios de varias líneas: llamados también comentarios de bloque. Son aquellos que comienzan con /* y terminan con */. Esta estructura implica que el texto que se escriban entre estos elementos será ignorado por el compilador de Kotlin.
