---
title: "StringBuilder"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una cadena mutable de caracteres."
type: docs
weight: 281
url: /es/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Representa una cadena mutable de caracteres. No puede ser extendida.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Inicializa una nueva instancia de la clase StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Inicializa una nueva instancia de la clase StringBuilder usando la capacidad especificada. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Inicializa una nueva instancia de la clase StringBuilder que comienza con una capacidad especificada y puede crecer hasta un máximo especificado. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Inicializa una nueva instancia de la clase StringBuilder usando la cadena especificada. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Inicializa una nueva instancia de la clase StringBuilder usando la cadena y la capacidad especificadas. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Inicializa una nueva instancia de la clase StringBuilder a partir de la subcadena y la capacidad especificadas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Agrega la representación en cadena de un valor booleano especificado a esta instancia. |
| [append(byte value)](#append-byte-) | Agrega la representación en cadena de un byte especificado a esta instancia. |
| [append(char value)](#append-char-) | Agrega la representación en cadena de un carácter Unicode especificado a esta instancia. |
| [append(char value, int repeatCount)](#append-char-int-) | Agrega un número especificado de copias de la representación en cadena de un carácter Unicode a esta instancia. |
| [append(char[] value)](#append-char---) | Agrega la representación en cadena de los caracteres Unicode en una matriz especificada a esta instancia. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Agrega la representación en cadena de un subarreglo especificado de caracteres Unicode a esta instancia. |
| [append(double value)](#append-double-) | Agrega la representación en cadena de un número double especificado a esta instancia. |
| [append(float value)](#append-float-) | Agrega la representación en cadena de un número float especificado a esta instancia. |
| [append(int value)](#append-int-) | Agrega la representación en cadena de un número int especificado a esta instancia. |
| [append(Object value)](#append-java.lang.Object-) | Agrega la representación en cadena de un objeto especificado a esta instancia. |
| [append(String value)](#append-java.lang.String-) | Agrega una copia de la cadena especificada a esta instancia. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Agrega una copia de una subcadena especificada a esta instancia. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Agrega la representación en cadena de un número BigDecimal especificado a esta instancia. |
| [append(long value)](#append-long-) | Agrega la representación en cadena de un número long especificado a esta instancia. |
| [append(short value)](#append-short-) | Agrega la representación en cadena de un número short especificado a esta instancia. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Agrega la cadena devuelta al procesar una cadena de formato compuesta, que contiene cero o más elementos de formato, a esta instancia. |
| [appendLine()](#appendLine--) | Agrega el terminador de línea predeterminado al final del objeto StringBuilder actual. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Agrega una copia de la cadena especificada seguida del terminador de línea predeterminado al final del objeto StringBuilder actual. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Copia los caracteres de un segmento especificado de esta instancia a un segmento especificado de una matriz Char de destino. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Garantiza que la capacidad de esta instancia de StringBuilder sea al menos el valor especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getCapacity()](#getCapacity--) | Obtiene el número máximo de caracteres que pueden almacenarse en la memoria asignada por la instancia actual. |
| [getLength()](#getLength--) | Obtiene la longitud del objeto StringBuilder actual. |
| [getMaxCapacity()](#getMaxCapacity--) | Obtiene la capacidad máxima de esta instancia. |
| [hashCode()](#hashCode--) | Devuelve un código hash para este StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Inserta la representación en cadena de un valor boolean en esta instancia en la posición de carácter especificada. |
| [insert(int index, byte value)](#insert-int-byte-) | Inserta la representación en cadena de un valor byte en esta instancia en la posición de carácter especificada. |
| [insert(int index, char value)](#insert-int-char-) | Inserta la representación en cadena de un carácter Unicode especificado en esta instancia en la posición de carácter especificada. |
| [insert(int index, char[] value)](#insert-int-char---) | Inserta la representación en cadena de una matriz especificada de caracteres Unicode en esta instancia en la posición de carácter especificada. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Inserta la representación en cadena de una submatriz especificada de caracteres Unicode en esta instancia en la posición de carácter especificada. |
| [insert(int index, double value)](#insert-int-double-) | Inserta la representación en cadena de un número double en esta instancia en la posición de carácter especificada. |
| [insert(int index, float value)](#insert-int-float-) | Inserta la representación en cadena de un número float en esta instancia en la posición de carácter especificada. |
| [insert(int index, int value)](#insert-int-int-) | Inserta la representación en cadena de un número int en esta instancia en la posición de carácter especificada. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserta la representación en cadena de un objeto en esta instancia en la posición de carácter especificada. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Inserta una cadena en esta instancia en la posición de carácter especificada. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Inserta una o más copias de una cadena especificada en esta instancia en la posición de carácter especificada. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Inserta la representación en cadena de un número decimal en esta instancia en la posición de carácter especificada. |
| [insert(int index, long value)](#insert-int-long-) | Inserta la representación en cadena de un número long en esta instancia en la posición de carácter especificada. |
| [insert(int index, short value)](#insert-int-short-) | Inserta la representación en cadena de un número short en esta instancia en la posición de carácter especificada. |
| [remove(int startIndex, int length)](#remove-int-int-) | Elimina el rango especificado de caracteres de esta instancia. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Reemplaza todas las apariciones de un carácter especificado en esta instancia con otro carácter especificado. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Reemplaza, dentro de una subcadena de esta instancia, todas las apariciones de un carácter especificado con otro carácter especificado. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Reemplaza todas las apariciones de una cadena especificada en esta instancia con otra cadena especificada. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Reemplaza, dentro de una subcadena de esta instancia, todas las apariciones de una cadena especificada con otra cadena especificada. |
| [setCapacity(int value)](#setCapacity-int-) | Establece el número máximo de caracteres que pueden estar contenidos en la memoria asignada por la instancia actual. |
| [setLength(int value)](#setLength-int-) | Establece la longitud del objeto StringBuilder actual. |
| [toString()](#toString--) | Convierte el valor de esta instancia a una cadena. |
| [toString(int startIndex, int length)](#toString-int-int-) | Convierte el valor de una subcadena de esta instancia a una cadena. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Inicializa una nueva instancia de la clase StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Inicializa una nueva instancia de la clase StringBuilder usando la capacidad especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| capacidad | int | El tamaño inicial sugerido de esta instancia. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Inicializa una nueva instancia de la clase StringBuilder que comienza con una capacidad especificada y puede crecer hasta un máximo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| capacidad | int | El tamaño inicial sugerido del StringBuilder. |
| maxCapacity | int | El número máximo de caracteres que la cadena actual puede contener. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Inicializa una nueva instancia de la clase StringBuilder usando la cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena utilizada para inicializar el valor de la instancia. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Inicializa una nueva instancia de la clase StringBuilder usando la cadena y la capacidad especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena utilizada para inicializar el valor de la instancia. |
| capacidad | int | El tamaño inicial sugerido del StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Inicializa una nueva instancia de la clase StringBuilder a partir de la subcadena y la capacidad especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena que contiene la subcadena utilizada para inicializar el valor de esta instancia. |
| startIndex | int | La posición dentro del valor donde comienza la subcadena. |
| longitud | int | El número de caracteres en la subcadena. |
| capacidad | int | El tamaño inicial sugerido del StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Agrega la representación en cadena de un valor booleano especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | El valor booleano a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Agrega la representación en cadena de un byte especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Agrega la representación en cadena de un carácter Unicode especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char | El carácter Unicode a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Agrega un número especificado de copias de la representación en cadena de un carácter Unicode a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char | El carácter a añadir. |
| repeatCount | int | El número de veces para añadir el valor. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Agrega la representación en cadena de los caracteres Unicode en una matriz especificada a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char[] | El arreglo de caracteres a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Agrega la representación en cadena de un subarreglo especificado de caracteres Unicode a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char[] | Un arreglo de caracteres. |
| startIndex | int | La posición inicial en el valor. |
| charCount | int | El número de caracteres a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Agrega la representación en cadena de un número double especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Agrega la representación en cadena de un número float especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Agrega la representación en cadena de un número int especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Agrega la representación en cadena de un objeto especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | El objeto a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Agrega una copia de la cadena especificada a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Agrega una copia de una subcadena especificada a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena que contiene la subcadena a añadir. |
| startIndex | int | La posición inicial de la subcadena dentro del valor. |
| count | int | El número de caracteres en el valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Agrega la representación en cadena de un número BigDecimal especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Agrega la representación en cadena de un número long especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | long | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Agrega la representación en cadena de un número short especificado a esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short | El valor a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Añade la cadena devuelta al procesar una cadena de formato compuesta, que contiene cero o más elementos de formato, a esta instancia. Cada elemento de formato se reemplaza por la representación en cadena de un argumento correspondiente en una matriz de parámetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | java.lang.String | Una cadena de formato compuesta. |
| args | java.lang.Object[] | Un arreglo de objetos para formatear. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Agrega el terminador de línea predeterminado al final del objeto StringBuilder actual.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Agrega una copia de la cadena especificada seguida del terminador de línea predeterminado al final del objeto StringBuilder actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | La cadena a añadir. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Copia los caracteres de un segmento especificado de esta instancia a un segmento especificado de una matriz Char de destino.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceIndex | int | La posición inicial en esta instancia desde donde se copiarán los caracteres. El índice comienza en cero. |
| destino | char[] | La matriz donde se copiarán los caracteres. |
| destinationIndex | int | La posición inicial en destination donde se copiarán los caracteres. El índice es basado en cero. |
| count | int | El número de caracteres a copiar. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Garantiza que la capacidad de esta instancia de StringBuilder sea al menos el valor especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| capacidad | int | La capacidad mínima a garantizar. |

**Returns:**
int - La nueva capacidad de esta instancia.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | Un objeto para comparar con esta instancia, o null. |

**Returns:**
boolean - true si esta instancia y sb tienen valores de string, Capacity y MaxCapacity iguales; de lo contrario, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Obtiene el número máximo de caracteres que pueden almacenarse en la memoria asignada por la instancia actual.

**Returns:**
int - El número máximo de caracteres que pueden estar contenidos en la memoria asignada por la instancia actual.
### getLength() {#getLength--}
```
public int getLength()
```


Obtiene la longitud del objeto StringBuilder actual.

**Returns:**
int - La longitud de esta instancia.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Obtiene la capacidad máxima de esta instancia.

**Returns:**
int - El número máximo de caracteres que esta instancia puede contener.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un código hash para este StringBuilder.

**Returns:**
int - Devuelve un valor de código hash para este objeto.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Inserta la representación en cadena de un valor boolean en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | boolean | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Inserta la representación en cadena de un valor byte en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | byte | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Inserta la representación en cadena de un carácter Unicode especificado en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | char | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Inserta la representación en cadena de una matriz especificada de caracteres Unicode en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | char[] | La matriz de caracteres a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Inserta la representación en cadena de una submatriz especificada de caracteres Unicode en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | char[] | Un arreglo de caracteres. |
| startIndex | int | El índice inicial dentro de value. |
| charCount | int | El número de caracteres a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Inserta la representación en cadena de un número double en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | double | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Inserta la representación en cadena de un número float en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | float | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Inserta la representación en cadena de un número int en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | int | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Inserta la representación en cadena de un objeto en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | java.lang.Object | El objeto a insertar, o null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Inserta una cadena en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | java.lang.String | La cadena a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Inserta una o más copias de una cadena especificada en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | java.lang.String | La cadena a insertar. |
| count | int | El número de veces para insertar value. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Inserta la representación en cadena de un número decimal en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | java.math.BigDecimal | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Inserta la representación en cadena de un número long en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | long | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Inserta la representación en cadena de un número short en esta instancia en la posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en esta instancia donde comienza la inserción. |
| valor | short | El valor a insertar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Elimina el rango especificado de caracteres de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | La posición basada en cero en esta instancia donde comienza la eliminación. |
| longitud | int | El número de caracteres a eliminar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Reemplaza todas las apariciones de un carácter especificado en esta instancia con otro carácter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldChar | char | El carácter a reemplazar. |
| newChar | char | El carácter que reemplaza oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Reemplaza, dentro de una subcadena de esta instancia, todas las apariciones de un carácter especificado con otro carácter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | char | El carácter a reemplazar. |
| newValue | char | El carácter que reemplaza oldChar. |
| startIndex | int | La posición en esta instancia donde comienza la subcadena. |
| count | int | La longitud de la subcadena. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Reemplaza todas las apariciones de una cadena especificada en esta instancia con otra cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | java.lang.String | La cadena a reemplazar. |
| newValue | java.lang.String | La cadena que reemplaza oldValue, o null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Reemplaza, dentro de una subcadena de esta instancia, todas las apariciones de una cadena especificada con otra cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | java.lang.String | La cadena a reemplazar. |
| newValue | java.lang.String | La cadena que reemplaza oldValue, o null. |
| startIndex | int | La posición en esta instancia donde comienza la subcadena. |
| count | int | La longitud de la subcadena. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Establece el número máximo de caracteres que pueden estar contenidos en la memoria asignada por la instancia actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | El número máximo de caracteres que pueden estar contenidos en la memoria asignada por la instancia actual. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Establece la longitud del objeto StringBuilder actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | La longitud de esta instancia. |

### toString() {#toString--}
```
public String toString()
```


Convierte el valor de esta instancia a una cadena.

**Returns:**
java.lang.String - Una cadena cuyo valor es el mismo que esta instancia.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Convierte el valor de una subcadena de esta instancia a una cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | La posición inicial de la subcadena en esta instancia. |
| longitud | int | La longitud de la subcadena. |

**Returns:**
java.lang.String - Una cadena cuyo valor es el mismo que la subcadena especificada de esta instancia.
