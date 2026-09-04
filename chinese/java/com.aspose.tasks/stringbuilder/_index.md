---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示可变的字符字符串。"
type: docs
weight: 281
url: /zh/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

表示可变的字符字符串。不能被扩展。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | 初始化 StringBuilder 类的新实例。 |
| [StringBuilder(int capacity)](#StringBuilder-int-) | 使用指定容量初始化 StringBuilder 类的新实例。 |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | 初始化 StringBuilder 类的新实例，该实例以指定容量开始，并且可以增长到指定的最大值。 |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | 使用指定字符串初始化 StringBuilder 类的新实例。 |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | 使用指定的字符串和容量初始化 StringBuilder 类的新实例。 |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | 从指定的子字符串和容量初始化 StringBuilder 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [append(boolean value)](#append-boolean-) | 将指定布尔值的字符串表示追加到此实例。 |
| [append(byte value)](#append-byte-) | 将指定字节的字符串表示追加到此实例。 |
| [append(char value)](#append-char-) | 将指定 Unicode 字符的字符串表示追加到此实例。 |
| [append(char value, int repeatCount)](#append-char-int-) | 将指定数量的 Unicode 字符的字符串表示副本追加到此实例。 |
| [append(char[] value)](#append-char---) | 将指定数组中 Unicode 字符的字符串表示追加到此实例。 |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | 将指定子数组中 Unicode 字符的字符串表示追加到此实例。 |
| [append(double value)](#append-double-) | 将指定 double 数字的字符串表示追加到此实例。 |
| [append(float value)](#append-float-) | 将指定 float 数字的字符串表示追加到此实例。 |
| [append(int value)](#append-int-) | 将指定 int 数字的字符串表示追加到此实例。 |
| [append(Object value)](#append-java.lang.Object-) | 将指定对象的字符串表示追加到此实例。 |
| [append(String value)](#append-java.lang.String-) | 将指定字符串的副本追加到此实例。 |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | 将指定子字符串的副本追加到此实例。 |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | 将指定 BigDecimal 数字的字符串表示追加到此实例。 |
| [append(long value)](#append-long-) | 将指定长整数的字符串表示追加到此实例。 |
| [append(short value)](#append-short-) | 将指定短整数的字符串表示追加到此实例。 |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | 将通过处理复合格式字符串（其中包含零个或多个格式项）返回的字符串追加到此实例。 |
| [appendLine()](#appendLine--) | 将默认行终止符追加到当前 StringBuilder 对象的末尾。 |
| [appendLine(String value)](#appendLine-java.lang.String-) | 将指定字符串的副本以及默认行终止符追加到当前 StringBuilder 对象的末尾。 |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | 将此实例的指定段中的字符复制到目标 Char 数组的指定段。 |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | 确保此 StringBuilder 实例的容量至少为指定值。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getCapacity()](#getCapacity--) | 获取当前实例分配的内存中可以容纳的最大字符数。 |
| [getLength()](#getLength--) | 获取当前 StringBuilder 对象的长度。 |
| [getMaxCapacity()](#getMaxCapacity--) | 获取此实例的最大容量。 |
| [hashCode()](#hashCode--) | 返回此 StringBuilder 的哈希码。 |
| [insert(int index, boolean value)](#insert-int-boolean-) | 在指定的字符位置将布尔值的字符串表示插入到此实例中。 |
| [insert(int index, byte value)](#insert-int-byte-) | 在指定的字符位置将字节值的字符串表示插入到此实例中。 |
| [insert(int index, char value)](#insert-int-char-) | 在指定的字符位置将指定的 Unicode 字符的字符串表示插入到此实例中。 |
| [insert(int index, char[] value)](#insert-int-char---) | 在指定的字符位置将指定的 Unicode 字符数组的字符串表示插入到此实例中。 |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | 在指定的字符位置将指定的 Unicode 子字符数组的字符串表示插入到此实例中。 |
| [insert(int index, double value)](#insert-int-double-) | 在指定的字符位置将 double 数的字符串表示插入到此实例中。 |
| [insert(int index, float value)](#insert-int-float-) | 在指定的字符位置将 float 数的字符串表示插入到此实例中。 |
| [insert(int index, int value)](#insert-int-int-) | 在指定的字符位置将 int 数的字符串表示插入到此实例中。 |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | 在指定的字符位置将对象的字符串表示插入到此实例中。 |
| [insert(int index, String value)](#insert-int-java.lang.String-) | 在指定的字符位置将字符串插入到此实例中。 |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | 在指定的字符位置将一个或多个指定字符串的副本插入到此实例中。 |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | 在指定的字符位置将 decimal 数的字符串表示插入到此实例中。 |
| [insert(int index, long value)](#insert-int-long-) | 在指定的字符位置将 long 数的字符串表示插入到此实例中。 |
| [insert(int index, short value)](#insert-int-short-) | 在指定的字符位置将 short 数的字符串表示插入到此实例中。 |
| [remove(int startIndex, int length)](#remove-int-int-) | 从此实例中移除指定范围的字符。 |
| [replace(char oldChar, char newChar)](#replace-char-char-) | 将此实例中指定字符的所有出现替换为另一个指定字符。 |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | 在此实例的子字符串中，将指定字符的所有出现替换为另一个指定字符。 |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 将此实例中指定字符串的所有出现替换为另一个指定字符串。 |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | 在此实例的子字符串中，将指定字符串的所有出现替换为另一个指定字符串。 |
| [setCapacity(int value)](#setCapacity-int-) | 设置当前实例分配的内存中可容纳的最大字符数。 |
| [setLength(int value)](#setLength-int-) | 设置当前 StringBuilder 对象的长度。 |
| [toString()](#toString--) | 将此实例的值转换为字符串。 |
| [toString(int startIndex, int length)](#toString-int-int-) | 将此实例的子字符串的值转换为字符串。 |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


初始化 StringBuilder 类的新实例。

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


使用指定容量初始化 StringBuilder 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 容量 | int | 此实例的建议起始大小。 |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


初始化 StringBuilder 类的新实例，该实例以指定容量开始，并且可以增长到指定的最大值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 容量 | int | StringBuilder 的建议起始大小。 |
| 最大容量 | int | 当前字符串可容纳的最大字符数。 |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


使用指定字符串初始化 StringBuilder 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于初始化实例值的字符串。 |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


使用指定的字符串和容量初始化 StringBuilder 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于初始化实例值的字符串。 |
| 容量 | int | StringBuilder 的建议起始大小。 |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


从指定的子字符串和容量初始化 StringBuilder 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 包含用于初始化此实例值的子字符串的字符串。 |
| 起始索引 | int | 值中子字符串开始的位置。 |
| 长度 | int | 子字符串中的字符数。 |
| 容量 | int | StringBuilder 的建议起始大小。 |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


将指定布尔值的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 要追加的布尔值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


将指定字节的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字节 | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


将指定 Unicode 字符的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字符 | 要追加的 Unicode 字符。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


将指定数量的 Unicode 字符的字符串表示副本追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字符 | 要追加的字符。 |
| repeatCount | int | 追加值的次数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


将指定数组中 Unicode 字符的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char[] | 要追加的字符数组。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


将指定子数组中 Unicode 字符的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char[] | 字符数组。 |
| 起始索引 | int | 值中的起始位置。 |
| charCount | int | 要追加的字符数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


将指定 double 数字的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


将指定 float 数字的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


将指定 int 数字的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


将指定对象的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 要追加的对象。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


将指定字符串的副本追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 要追加的字符串。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


将指定子字符串的副本追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 包含要追加子字符串的字符串。 |
| 起始索引 | int | 值中子字符串的起始位置。 |
| count | int | 要在值中追加的字符数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


将指定 BigDecimal 数字的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


将指定长整数的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | long | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


将指定短整数的字符串表示追加到此实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | short | 要追加的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


将通过处理复合格式字符串（其中包含零个或多个格式项）返回的字符串追加到此实例。每个格式项都会被参数数组中相应参数的字符串表示替代。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | java.lang.String | 复合格式字符串。 |
| args | java.lang.Object[] | 用于格式化的对象数组。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


将默认行终止符追加到当前 StringBuilder 对象的末尾。

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


将指定字符串的副本以及默认行终止符追加到当前 StringBuilder 对象的末尾。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 要追加的字符串。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


将此实例的指定段中的字符复制到目标 Char 数组的指定段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceIndex | int | 此实例中字符将被复制的起始位置。索引从零开始。 |
| 目标 | char[] | 字符将被复制的数组。 |
| 目标索引 | int | 在目标中字符将被复制的起始位置。索引从零开始。 |
| count | int | 要复制的字符数。 |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


确保此 StringBuilder 实例的容量至少为指定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 容量 | int | 要确保的最小容量。 |

**Returns:**
int - 此实例的新容量。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象，或 null。 |

**Returns:**
boolean - 如果此实例和 sb 的字符串、Capacity 和 MaxCapacity 值相等则为 true；否则为 false。
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


获取当前实例分配的内存中可以容纳的最大字符数。

**Returns:**
int - 当前实例分配的内存中可以容纳的最大字符数。
### getLength() {#getLength--}
```
public int getLength()
```


获取当前 StringBuilder 对象的长度。

**Returns:**
int - 此实例的长度。
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


获取此实例的最大容量。

**Returns:**
int - 此实例可以容纳的最大字符数。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回此 StringBuilder 的哈希码。

**Returns:**
int - 返回此对象的哈希码值。
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


在指定的字符位置将布尔值的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | boolean | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


在指定的字符位置将字节值的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | 字节 | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


在指定的字符位置将指定的 Unicode 字符的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | 字符 | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


在指定的字符位置将指定的 Unicode 字符数组的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | char[] | 要插入的字符数组。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


在指定的字符位置将指定的 Unicode 子字符数组的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | char[] | 字符数组。 |
| 起始索引 | int | value 中的起始索引。 |
| charCount | int | 要插入的字符数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


在指定的字符位置将 double 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | double | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


在指定的字符位置将 float 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | float | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


在指定的字符位置将 int 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | int | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


在指定的字符位置将对象的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | java.lang.Object | 要插入的对象，或 null。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


在指定的字符位置将字符串插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | java.lang.String | 要插入的字符串。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


在指定的字符位置将一个或多个指定字符串的副本插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | java.lang.String | 要插入的字符串。 |
| count | int | 插入 value 的次数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


在指定的字符位置将 decimal 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | java.math.BigDecimal | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


在指定的字符位置将 long 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | long | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


在指定的字符位置将 short 数的字符串表示插入到此实例中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此实例中插入开始的位置。 |
| 值 | short | 要插入的值。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


从此实例中移除指定范围的字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 起始索引 | int | 此实例中删除开始的零基位置。 |
| 长度 | int | 要删除的字符数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


将此实例中指定字符的所有出现替换为另一个指定字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 旧字符 | 字符 | 要替换的字符。 |
| 新字符 | 字符 | 替换 oldChar 的字符。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


在此实例的子字符串中，将指定字符的所有出现替换为另一个指定字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | 字符 | 要替换的字符。 |
| newValue | 字符 | 替换 oldChar 的字符。 |
| 起始索引 | int | 此实例中子字符串开始的位置。 |
| count | int | 子字符串的长度。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


将此实例中指定字符串的所有出现替换为另一个指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | java.lang.String | 要替换的字符串。 |
| newValue | java.lang.String | 替换 oldValue 的字符串，或 null。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


在此实例的子字符串中，将指定字符串的所有出现替换为另一个指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | java.lang.String | 要替换的字符串。 |
| newValue | java.lang.String | 替换 oldValue 的字符串，或 null。 |
| 起始索引 | int | 此实例中子字符串开始的位置。 |
| count | int | 子字符串的长度。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


设置当前实例分配的内存中可容纳的最大字符数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 当前实例分配的内存中可以容纳的最大字符数。 |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


设置当前 StringBuilder 对象的长度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 此实例的长度。 |

### toString() {#toString--}
```
public String toString()
```


将此实例的值转换为字符串。

**Returns:**
java.lang.String - 与此实例值相同的字符串。
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


将此实例的子字符串的值转换为字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 起始索引 | int | 此实例中子字符串的起始位置。 |
| 长度 | int | 子字符串的长度。 |

**Returns:**
java.lang.String - 与此实例指定子字符串的值相同的字符串。
