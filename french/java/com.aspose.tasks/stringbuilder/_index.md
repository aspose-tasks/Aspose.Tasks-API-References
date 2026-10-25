---
title: "StringBuilder"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une chaîne de caractères mutable."
type: docs
weight: 281
url: /fr/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Représente une chaîne mutable de caractères. Ne peut pas être étendue.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Initialise une nouvelle instance de la classe StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Initialise une nouvelle instance de la classe StringBuilder en utilisant la capacité spécifiée. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Initialise une nouvelle instance de la classe StringBuilder qui commence avec une capacité spécifiée et peut croître jusqu'à un maximum spécifié. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Initialise une nouvelle instance de la classe StringBuilder en utilisant la chaîne spécifiée. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Initialise une nouvelle instance de la classe StringBuilder en utilisant la chaîne et la capacité spécifiées. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Initialise une nouvelle instance de la classe StringBuilder à partir de la sous-chaîne et de la capacité spécifiées. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Ajoute la représentation sous forme de chaîne d'une valeur booléenne spécifiée à cette instance. |
| [append(byte value)](#append-byte-) | Ajoute la représentation sous forme de chaîne d'un octet spécifié à cette instance. |
| [append(char value)](#append-char-) | Ajoute la représentation sous forme de chaîne d'un caractère Unicode spécifié à cette instance. |
| [append(char value, int repeatCount)](#append-char-int-) | Ajoute un nombre spécifié de copies de la représentation sous forme de chaîne d'un caractère Unicode à cette instance. |
| [append(char[] value)](#append-char---) | Ajoute la représentation sous forme de chaîne des caractères Unicode d'un tableau spécifié à cette instance. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Ajoute la représentation sous forme de chaîne d'un sous-tableau spécifié de caractères Unicode à cette instance. |
| [append(double value)](#append-double-) | Ajoute la représentation sous forme de chaîne d'un nombre double spécifié à cette instance. |
| [append(float value)](#append-float-) | Ajoute la représentation sous forme de chaîne d'un nombre flottant spécifié à cette instance. |
| [append(int value)](#append-int-) | Ajoute la représentation sous forme de chaîne d'un nombre entier spécifié à cette instance. |
| [append(Object value)](#append-java.lang.Object-) | Ajoute la représentation sous forme de chaîne d'un objet spécifié à cette instance. |
| [append(String value)](#append-java.lang.String-) | Ajoute une copie de la chaîne spécifiée à cette instance. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Ajoute une copie d'une sous-chaîne spécifiée à cette instance. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Ajoute la représentation sous forme de chaîne d'un nombre BigDecimal spécifié à cette instance. |
| [append(long value)](#append-long-) | Ajoute la représentation sous forme de chaîne d'un nombre long spécifié à cette instance. |
| [append(short value)](#append-short-) | Ajoute la représentation sous forme de chaîne d'un nombre court spécifié à cette instance. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Ajoute la chaîne renvoyée par le traitement d'une chaîne de format composite, qui contient zéro ou plusieurs éléments de format, à cette instance. |
| [appendLine()](#appendLine--) | Ajoute le séparateur de ligne par défaut à la fin de l'objet StringBuilder actuel. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Ajoute une copie de la chaîne spécifiée suivie du séparateur de ligne par défaut à la fin de l'objet StringBuilder actuel. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Copie les caractères d'un segment spécifié de cette instance vers un segment spécifié d'un tableau Char de destination. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Garantit que la capacité de cette instance de StringBuilder est au moins la valeur spécifiée. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getCapacity()](#getCapacity--) | Obtient le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle. |
| [getLength()](#getLength--) | Obtient la longueur de l'objet StringBuilder actuel. |
| [getMaxCapacity()](#getMaxCapacity--) | Obtient la capacité maximale de cette instance. |
| [hashCode()](#hashCode--) | Renvoie un code de hachage pour ce StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Insère la représentation sous forme de chaîne d'une valeur booléenne dans cette instance à la position de caractère spécifiée. |
| [insert(int index, byte value)](#insert-int-byte-) | Insère la représentation sous forme de chaîne d'une valeur byte dans cette instance à la position de caractère spécifiée. |
| [insert(int index, char value)](#insert-int-char-) | Insère la représentation sous forme de chaîne d'un caractère Unicode spécifié dans cette instance à la position de caractère spécifiée. |
| [insert(int index, char[] value)](#insert-int-char---) | Insère la représentation sous forme de chaîne d'un tableau spécifié de caractères Unicode dans cette instance à la position de caractère spécifiée. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Insère la représentation sous forme de chaîne d'une sous‑section spécifiée de caractères Unicode dans cette instance à la position de caractère spécifiée. |
| [insert(int index, double value)](#insert-int-double-) | Insère la représentation sous forme de chaîne d'un nombre double dans cette instance à la position de caractère spécifiée. |
| [insert(int index, float value)](#insert-int-float-) | Insère la représentation sous forme de chaîne d'un nombre flottant dans cette instance à la position de caractère spécifiée. |
| [insert(int index, int value)](#insert-int-int-) | Insère la représentation sous forme de chaîne d'un nombre entier (int) dans cette instance à la position de caractère spécifiée. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Insère la représentation sous forme de chaîne d'un objet dans cette instance à la position de caractère spécifiée. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Insère une chaîne dans cette instance à la position de caractère spécifiée. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Insère une ou plusieurs copies d'une chaîne spécifiée dans cette instance à la position de caractère spécifiée. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Insère la représentation sous forme de chaîne d'un nombre décimal dans cette instance à la position de caractère spécifiée. |
| [insert(int index, long value)](#insert-int-long-) | Insère la représentation sous forme de chaîne d'un nombre long dans cette instance à la position de caractère spécifiée. |
| [insert(int index, short value)](#insert-int-short-) | Insère la représentation sous forme de chaîne d'un nombre court dans cette instance à la position de caractère spécifiée. |
| [remove(int startIndex, int length)](#remove-int-int-) | Supprime la plage de caractères spécifiée de cette instance. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Remplace toutes les occurrences d'un caractère spécifié dans cette instance par un autre caractère spécifié. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Remplace, au sein d'une sous-chaîne de cette instance, toutes les occurrences d'un caractère spécifié par un autre caractère spécifié. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Remplace toutes les occurrences d'une chaîne spécifiée dans cette instance par une autre chaîne spécifiée. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Remplace, au sein d'une sous-chaîne de cette instance, toutes les occurrences d'une chaîne spécifiée par une autre chaîne spécifiée. |
| [setCapacity(int value)](#setCapacity-int-) | Définit le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle. |
| [setLength(int value)](#setLength-int-) | Définit la longueur de l'objet StringBuilder actuel. |
| [toString()](#toString--) | Convertit la valeur de cette instance en chaîne. |
| [toString(int startIndex, int length)](#toString-int-int-) | Convertit la valeur d'une sous-chaîne de cette instance en chaîne. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Initialise une nouvelle instance de la classe StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Initialise une nouvelle instance de la classe StringBuilder en utilisant la capacité spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| capacité | int | La taille de départ suggérée pour cette instance. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Initialise une nouvelle instance de la classe StringBuilder qui commence avec une capacité spécifiée et peut croître jusqu'à un maximum spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| capacité | int | La taille de départ suggérée pour le StringBuilder. |
| maxCapacity | int | Le nombre maximal de caractères que la chaîne actuelle peut contenir. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Initialise une nouvelle instance de la classe StringBuilder en utilisant la chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne utilisée pour initialiser la valeur de l'instance. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Initialise une nouvelle instance de la classe StringBuilder en utilisant la chaîne et la capacité spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne utilisée pour initialiser la valeur de l'instance. |
| capacité | int | La taille de départ suggérée pour le StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Initialise une nouvelle instance de la classe StringBuilder à partir de la sous-chaîne et de la capacité spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne qui contient la sous-chaîne utilisée pour initialiser la valeur de cette instance. |
| startIndex | int | La position dans la valeur où commence la sous-chaîne. |
| longueur | int | Le nombre de caractères dans la sous-chaîne. |
| capacité | int | La taille de départ suggérée pour le StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Ajoute la représentation sous forme de chaîne d'une valeur booléenne spécifiée à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | La valeur booléenne à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Ajoute la représentation sous forme de chaîne d'un octet spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Ajoute la représentation sous forme de chaîne d'un caractère Unicode spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char | Le caractère Unicode à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Ajoute un nombre spécifié de copies de la représentation sous forme de chaîne d'un caractère Unicode à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char | Le caractère à ajouter. |
| repeatCount | int | Le nombre de fois d'ajouter la valeur. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Ajoute la représentation sous forme de chaîne des caractères Unicode d'un tableau spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char[] | Le tableau de caractères à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Ajoute la représentation sous forme de chaîne d'un sous-tableau spécifié de caractères Unicode à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char[] | Un tableau de caractères. |
| startIndex | int | La position de départ dans la valeur. |
| charCount | int | Le nombre de caractères à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Ajoute la représentation sous forme de chaîne d'un nombre double spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Ajoute la représentation sous forme de chaîne d'un nombre flottant spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Ajoute la représentation sous forme de chaîne d'un nombre entier spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Ajoute la représentation sous forme de chaîne d'un objet spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | L'objet à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Ajoute une copie de la chaîne spécifiée à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Ajoute une copie d'une sous-chaîne spécifiée à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne qui contient la sous-chaîne à ajouter. |
| startIndex | int | La position de départ de la sous-chaîne dans la valeur. |
| count | int | Le nombre de caractères dans la valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Ajoute la représentation sous forme de chaîne d'un nombre BigDecimal spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Ajoute la représentation sous forme de chaîne d'un nombre long spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | long | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Ajoute la représentation sous forme de chaîne d'un nombre court spécifié à cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short | La valeur à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Ajoute la chaîne renvoyée par le traitement d'une chaîne de format composite, qui contient zéro ou plusieurs éléments de format, à cette instance. Chaque élément de format est remplacé par la représentation sous forme de chaîne d'un argument correspondant dans un tableau de paramètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | java.lang.String | Une chaîne de format composite. |
| args | java.lang.Object[] | Un tableau d'objets à formater. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Ajoute le séparateur de ligne par défaut à la fin de l'objet StringBuilder actuel.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Ajoute une copie de la chaîne spécifiée suivie du séparateur de ligne par défaut à la fin de l'objet StringBuilder actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La chaîne à ajouter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Copie les caractères d'un segment spécifié de cette instance vers un segment spécifié d'un tableau Char de destination.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | int | La position de départ dans cette instance d'où les caractères seront copiés. L'index commence à zéro. |
| destination | char[] | Le tableau où les caractères seront copiés. |
| destinationIndex | int | La position de départ dans destination où les caractères seront copiés. L'index commence à zéro. |
| count | int | Le nombre de caractères à copier. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Garantit que la capacité de cette instance de StringBuilder est au moins la valeur spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| capacité | int | La capacité minimale à garantir. |

**Returns:**
int - La nouvelle capacité de cette instance.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | Un objet à comparer avec cette instance, ou null. |

**Returns:**
boolean - true si cette instance et sb ont des valeurs égales pour string, Capacity et MaxCapacity ; sinon, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Obtient le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle.

**Returns:**
int - Le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle.
### getLength() {#getLength--}
```
public int getLength()
```


Obtient la longueur de l'objet StringBuilder actuel.

**Returns:**
int - La longueur de cette instance.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Obtient la capacité maximale de cette instance.

**Returns:**
int - Le nombre maximal de caractères que cette instance peut contenir.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie un code de hachage pour ce StringBuilder.

**Returns:**
int - Retourne une valeur de code de hachage pour cet objet.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Insère la représentation sous forme de chaîne d'une valeur booléenne dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | booléen | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Insère la représentation sous forme de chaîne d'une valeur byte dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | byte | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Insère la représentation sous forme de chaîne d'un caractère Unicode spécifié dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | char | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Insère la représentation sous forme de chaîne d'un tableau spécifié de caractères Unicode dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | char[] | Le tableau de caractères à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Insère la représentation sous forme de chaîne d'une sous‑section spécifiée de caractères Unicode dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | char[] | Un tableau de caractères. |
| startIndex | int | L'index de départ dans value. |
| charCount | int | Le nombre de caractères à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Insère la représentation sous forme de chaîne d'un nombre double dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | double | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Insère la représentation sous forme de chaîne d'un nombre flottant dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | float | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Insère la représentation sous forme de chaîne d'un nombre entier (int) dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | int | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Insère la représentation sous forme de chaîne d'un objet dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | java.lang.Object | L'objet à insérer, ou null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Insère une chaîne dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | java.lang.String | La chaîne à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Insère une ou plusieurs copies d'une chaîne spécifiée dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | java.lang.String | La chaîne à insérer. |
| count | int | Le nombre de fois d'insérer value. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Insère la représentation sous forme de chaîne d'un nombre décimal dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | java.math.BigDecimal | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Insère la représentation sous forme de chaîne d'un nombre long dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | long | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Insère la représentation sous forme de chaîne d'un nombre court dans cette instance à la position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | La position dans cette instance où l'insertion commence. |
| valeur | short | La valeur à insérer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Supprime la plage de caractères spécifiée de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | La position basée sur zéro dans cette instance où la suppression commence. |
| longueur | int | Le nombre de caractères à supprimer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Remplace toutes les occurrences d'un caractère spécifié dans cette instance par un autre caractère spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldChar | char | Le caractère à remplacer. |
| newChar | char | Le caractère qui remplace oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Remplace, au sein d'une sous-chaîne de cette instance, toutes les occurrences d'un caractère spécifié par un autre caractère spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | char | Le caractère à remplacer. |
| newValue | char | Le caractère qui remplace oldChar. |
| startIndex | int | La position dans cette instance où commence la sous-chaîne. |
| count | int | La longueur de la sous-chaîne. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Remplace toutes les occurrences d'une chaîne spécifiée dans cette instance par une autre chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | La chaîne à remplacer. |
| newValue | java.lang.String | La chaîne qui remplace oldValue, ou null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Remplace, au sein d'une sous-chaîne de cette instance, toutes les occurrences d'une chaîne spécifiée par une autre chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | La chaîne à remplacer. |
| newValue | java.lang.String | La chaîne qui remplace oldValue, ou null. |
| startIndex | int | La position dans cette instance où commence la sous-chaîne. |
| count | int | La longueur de la sous-chaîne. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Définit le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | Le nombre maximal de caractères pouvant être contenus dans la mémoire allouée par l'instance actuelle. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Définit la longueur de l'objet StringBuilder actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | La longueur de cette instance. |

### toString() {#toString--}
```
public String toString()
```


Convertit la valeur de cette instance en chaîne.

**Returns:**
java.lang.String - Une chaîne dont la valeur est identique à cette instance.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Convertit la valeur d'une sous-chaîne de cette instance en chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | La position de départ de la sous-chaîne dans cette instance. |
| longueur | int | La longueur de la sous-chaîne. |

**Returns:**
java.lang.String - Une chaîne dont la valeur est identique à la sous-chaîne spécifiée de cette instance.
