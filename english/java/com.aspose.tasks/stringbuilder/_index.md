---
title: StringBuilder
second_title: Aspose.Tasks for Java API Reference
description: Represents a mutable string of characters.
type: docs
weight: 280
url: /java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Represents a mutable string of characters. Cannot be extended.
## Constructors

| Constructor | Description |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Initializes a new instance of the StringBuilder class. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Initializes a new instance of the StringBuilder class using the specified capacity. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Initializes a new instance of the StringBuilder class that starts with a specified capacity and can grow to a specified maximum. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Initializes a new instance of the StringBuilder class using the specified string. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Initializes a new instance of the StringBuilder class using the specified string and capacity. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Initializes a new instance of the StringBuilder class from the specified substring and capacity. |
## Methods

| Method | Description |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Appends the string representation of a specified boolean value to this instance. |
| [append(byte value)](#append-byte-) | Appends the string representation of a specified byte to this instance. |
| [append(char value)](#append-char-) | Appends the string representation of a specified Unicode character to this instance. |
| [append(char value, int repeatCount)](#append-char-int-) | Appends a specified number of copies of the string representation of a Unicode character to this instance. |
| [append(char[] value)](#append-char---) | Appends the string representation of the Unicode characters in a specified array to this instance. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Appends the string representation of a specified subarray of Unicode characters to this instance. |
| [append(double value)](#append-double-) | Appends the string representation of a specified double number to this instance. |
| [append(float value)](#append-float-) | Appends the string representation of a specified float number to this instance. |
| [append(int value)](#append-int-) | Appends the string representation of a specified int number to this instance. |
| [append(Object value)](#append-java.lang.Object-) | Appends the string representation of a specified object to this instance. |
| [append(String value)](#append-java.lang.String-) | Appends a copy of the specified string to this instance. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Appends a copy of a specified substring to this instance. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Appends the string representation of a specified BigDecimal number to this instance. |
| [append(long value)](#append-long-) | Appends the string representation of a specified long number to this instance. |
| [append(short value)](#append-short-) | Appends the string representation of a specified short number to this instance. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Appends the string returned by processing a composite format string, which contains zero or more format items, to this instance. |
| [appendLine()](#appendLine--) | Appends the default line terminator to the end of the current StringBuilder object. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Appends a copy of the specified string followed by the default line terminator to the end of the current StringBuilder object. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Copies the characters from a specified segment of this instance to a specified segment of a destination Char array. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Ensures that the capacity of this instance of StringBuilder is at least the specified value. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getCapacity()](#getCapacity--) | Gets the maximum number of characters that can be contained in the memory allocated by the current instance. |
| [getLength()](#getLength--) | Gets the length of the current StringBuilder object. |
| [getMaxCapacity()](#getMaxCapacity--) | Gets the maximum capacity of this instance. |
| [hashCode()](#hashCode--) | Returns a hash code for this StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Inserts the string representation of a boolean value into this instance at the specified character position. |
| [insert(int index, byte value)](#insert-int-byte-) | Inserts the string representation of a byte value into this instance at the specified character position. |
| [insert(int index, char value)](#insert-int-char-) | Inserts the string representation of a specified Unicode character into this instance at the specified character position. |
| [insert(int index, char[] value)](#insert-int-char---) | Inserts the string representation of a specified array of Unicode characters into this instance at the specified character position. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Inserts the string representation of a specified subarray of Unicode characters into this instance at the specified character position. |
| [insert(int index, double value)](#insert-int-double-) | Inserts the string representation of a double number into this instance at the specified character position. |
| [insert(int index, float value)](#insert-int-float-) | Inserts the string representation of a float number into this instance at the specified character position. |
| [insert(int index, int value)](#insert-int-int-) | Inserts the string representation of an int number into this instance at the specified character position. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserts the string representation of an object into this instance at the specified character position. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Inserts a string into this instance at the specified character position. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Inserts one or more copies of a specified string into this instance at the specified character position. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Inserts the string representation of a decimal number into this instance at the specified character position. |
| [insert(int index, long value)](#insert-int-long-) | Inserts the string representation of a long number into this instance at the specified character position. |
| [insert(int index, short value)](#insert-int-short-) | Inserts the string representation of a short number into this instance at the specified character position. |
| [remove(int startIndex, int length)](#remove-int-int-) | Removes the specified range of characters from this instance. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Replaces all occurrences of a specified character in this instance with another specified character. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Replaces, within a substring of this instance, all occurrences of a specified character with another specified character. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Replaces all occurrences of a specified string in this instance with another specified string. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Replaces, within a substring of this instance, all occurrences of a specified string with another specified string. |
| [setCapacity(int value)](#setCapacity-int-) | Sets the maximum number of characters that can be contained in the memory allocated by the current instance. |
| [setLength(int value)](#setLength-int-) | Sets the length of the current StringBuilder object. |
| [toString()](#toString--) | Converts the value of this instance to a String. |
| [toString(int startIndex, int length)](#toString-int-int-) | Converts the value of a substring of this instance to a String. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Initializes a new instance of the StringBuilder class.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Initializes a new instance of the StringBuilder class using the specified capacity.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| capacity | int | The suggested starting size of this instance. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Initializes a new instance of the StringBuilder class that starts with a specified capacity and can grow to a specified maximum.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| capacity | int | The suggested starting size of the StringBuilder. |
| maxCapacity | int | The maximum number of characters the current string can contain. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Initializes a new instance of the StringBuilder class using the specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string used to initialize the value of the instance. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Initializes a new instance of the StringBuilder class using the specified string and capacity.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string used to initialize the value of the instance. |
| capacity | int | The suggested starting size of the StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Initializes a new instance of the StringBuilder class from the specified substring and capacity.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string that contains the substring used to initialize the value of this instance. |
| startIndex | int | The position within value where the substring begins. |
| length | int | The number of characters in the substring. |
| capacity | int | The suggested starting size of the StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Appends the string representation of a specified boolean value to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The boolean value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Appends the string representation of a specified byte to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Appends the string representation of a specified Unicode character to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The Unicode character to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Appends a specified number of copies of the string representation of a Unicode character to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The character to append. |
| repeatCount | int | The number of times to append value. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Appends the string representation of the Unicode characters in a specified array to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char[] | The array of characters to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Appends the string representation of a specified subarray of Unicode characters to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char[] | A character array. |
| startIndex | int | The starting position in value. |
| charCount | int | The number of characters to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Appends the string representation of a specified double number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Appends the string representation of a specified float number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Appends the string representation of a specified int number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Appends the string representation of a specified object to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | The object to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Appends a copy of the specified string to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Appends a copy of a specified substring to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string that contains the substring to append. |
| startIndex | int | The starting position of the substring within value. |
| count | int | The number of characters in value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Appends the string representation of a specified BigDecimal number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Appends the string representation of a specified long number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | long | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Appends the string representation of a specified short number to this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short | The value to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Appends the string returned by processing a composite format string, which contains zero or more format items, to this instance. Each format item is replaced by the string representation of a corresponding argument in a parameter array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | java.lang.String | A composite format string. |
| args | java.lang.Object[] | An array of objects to format. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Appends the default line terminator to the end of the current StringBuilder object.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Appends a copy of the specified string followed by the default line terminator to the end of the current StringBuilder object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string to append. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Copies the characters from a specified segment of this instance to a specified segment of a destination Char array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The starting position in this instance where characters will be copied from. The index is zero-based. |
| destination | char[] | The array where characters will be copied. |
| destinationIndex | int | The starting position in destination where characters will be copied. The index is zero-based. |
| count | int | The number of characters to be copied. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Ensures that the capacity of this instance of StringBuilder is at least the specified value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| capacity | int | The minimum capacity to ensure. |

**Returns:**
int - The new capacity of this instance.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | An object to compare with this instance, or null. |

**Returns:**
boolean - true if this instance and sb have equal string, Capacity, and MaxCapacity values; otherwise, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Gets the maximum number of characters that can be contained in the memory allocated by the current instance.

**Returns:**
int - The maximum number of characters that can be contained in the memory allocated by the current instance.
### getLength() {#getLength--}
```
public int getLength()
```


Gets the length of the current StringBuilder object.

**Returns:**
int - The length of this instance.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Gets the maximum capacity of this instance.

**Returns:**
int - The maximum number of characters this instance can hold.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for this StringBuilder.

**Returns:**
int - Returns a hash code value for this object.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Inserts the string representation of a boolean value into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | boolean | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Inserts the string representation of a byte value into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | byte | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Inserts the string representation of a specified Unicode character into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | char | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Inserts the string representation of a specified array of Unicode characters into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | char[] | The character array to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Inserts the string representation of a specified subarray of Unicode characters into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | char[] | A character array. |
| startIndex | int | The starting index within value. |
| charCount | int | The number of characters to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Inserts the string representation of a double number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | double | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Inserts the string representation of a float number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | float | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Inserts the string representation of an int number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | int | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Inserts the string representation of an object into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | java.lang.Object | The object to insert, or null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Inserts a string into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | java.lang.String | The string to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Inserts one or more copies of a specified string into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | java.lang.String | The string to insert. |
| count | int | The number of times to insert value. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Inserts the string representation of a decimal number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | java.math.BigDecimal | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Inserts the string representation of a long number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | long | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Inserts the string representation of a short number into this instance at the specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in this instance where insertion begins. |
| value | short | The value to insert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Removes the specified range of characters from this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The zero-based position in this instance where removal begins. |
| length | int | The number of characters to remove. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Replaces all occurrences of a specified character in this instance with another specified character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChar | char | The character to replace. |
| newChar | char | The character that replaces oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Replaces, within a substring of this instance, all occurrences of a specified character with another specified character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | char | The character to replace. |
| newValue | char | The character that replaces oldChar. |
| startIndex | int | The position in this instance where the substring begins. |
| count | int | The length of the substring. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Replaces all occurrences of a specified string in this instance with another specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | The string to replace. |
| newValue | java.lang.String | The string that replaces oldValue, or null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Replaces, within a substring of this instance, all occurrences of a specified string with another specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | The string to replace. |
| newValue | java.lang.String | The string that replaces oldValue, or null. |
| startIndex | int | The position in this instance where the substring begins. |
| count | int | The length of the substring. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Sets the maximum number of characters that can be contained in the memory allocated by the current instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of characters that can be contained in the memory allocated by the current instance. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Sets the length of the current StringBuilder object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The length of this instance. |

### toString() {#toString--}
```
public String toString()
```


Converts the value of this instance to a String.

**Returns:**
java.lang.String - A string whose value is the same as this instance.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Converts the value of a substring of this instance to a String.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The starting position of the substring in this instance. |
| length | int | The length of the substring. |

**Returns:**
java.lang.String - A string whose value is the same as the specified substring of this instance.
