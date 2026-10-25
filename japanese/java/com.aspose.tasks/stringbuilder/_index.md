---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "可変の文字列を表します。"
type: docs
weight: 281
url: /ja/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

可変の文字列を表します。拡張できません。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | StringBuilder クラスの新しいインスタンスを初期化します。 |
| [StringBuilder(int capacity)](#StringBuilder-int-) | 指定された容量を使用して、StringBuilder クラスの新しいインスタンスを初期化します。 |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | 指定された容量で開始し、指定された最大値まで拡張できる StringBuilder クラスの新しいインスタンスを初期化します。 |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | 指定された文字列を使用して、StringBuilder クラスの新しいインスタンスを初期化します。 |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | 指定された文字列と容量を使用して、StringBuilder クラスの新しいインスタンスを初期化します。 |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | 指定されたサブ文字列と容量から、StringBuilder クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [append(boolean value)](#append-boolean-) | 指定されたブール値の文字列表現をこのインスタンスに追加します。 |
| [append(byte value)](#append-byte-) | 指定されたバイトの文字列表現をこのインスタンスに追加します。 |
| [append(char value)](#append-char-) | 指定された Unicode 文字の文字列表現をこのインスタンスに追加します。 |
| [append(char value, int repeatCount)](#append-char-int-) | Unicode 文字の文字列表現の指定された回数分のコピーをこのインスタンスに追加します。 |
| [append(char[] value)](#append-char---) | 指定された配列内の Unicode 文字の文字列表現をこのインスタンスに追加します。 |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | 指定された Unicode 文字のサブ配列の文字列表現をこのインスタンスに追加します。 |
| [append(double value)](#append-double-) | 指定された double 数値の文字列表現をこのインスタンスに追加します。 |
| [append(float value)](#append-float-) | 指定された float 数値の文字列表現をこのインスタンスに追加します。 |
| [append(int value)](#append-int-) | 指定された int 数値の文字列表現をこのインスタンスに追加します。 |
| [append(Object value)](#append-java.lang.Object-) | 指定されたオブジェクトの文字列表現をこのインスタンスに追加します。 |
| [append(String value)](#append-java.lang.String-) | 指定された文字列のコピーをこのインスタンスに追加します。 |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | 指定されたサブ文字列のコピーをこのインスタンスに追加します。 |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | 指定された BigDecimal 数値の文字列表現をこのインスタンスに追加します。 |
| [append(long value)](#append-long-) | 指定された long 数の文字列表現をこのインスタンスに追加します。 |
| [append(short value)](#append-short-) | 指定された short 数の文字列表現をこのインスタンスに追加します。 |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | 0 個以上の書式項目を含む複合書式文字列を処理して返される文字列をこのインスタンスに追加します。 |
| [appendLine()](#appendLine--) | 現在の StringBuilder オブジェクトの末尾にデフォルトの改行文字を追加します。 |
| [appendLine(String value)](#appendLine-java.lang.String-) | 指定された文字列のコピーとデフォルトの改行文字を続けて、現在の StringBuilder オブジェクトの末尾に追加します。 |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | このインスタンスの指定されたセグメントから文字をコピーし、宛先 Char 配列の指定されたセグメントへ配置します。 |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | この StringBuilder インスタンスの容量が指定された値以上であることを保証します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getCapacity()](#getCapacity--) | 現在のインスタンスが割り当てたメモリに格納できる最大文字数を取得します。 |
| [getLength()](#getLength--) | 現在の StringBuilder オブジェクトの長さを取得します。 |
| [getMaxCapacity()](#getMaxCapacity--) | このインスタンスの最大容量を取得します。 |
| [hashCode()](#hashCode--) | この StringBuilder のハッシュコードを返します。 |
| [insert(int index, boolean value)](#insert-int-boolean-) | 指定された文字位置に boolean 値の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, byte value)](#insert-int-byte-) | 指定された文字位置に byte 値の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, char value)](#insert-int-char-) | 指定された文字位置に指定された Unicode 文字の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, char[] value)](#insert-int-char---) | 指定された文字位置に指定された Unicode 文字配列の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | 指定された文字位置に指定された Unicode 文字サブ配列の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, double value)](#insert-int-double-) | 指定された文字位置に double 数の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, float value)](#insert-int-float-) | 指定された文字位置に float 数の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, int value)](#insert-int-int-) | 指定された文字位置に int 数の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | 指定された文字位置にオブジェクトの文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, String value)](#insert-int-java.lang.String-) | 指定された文字位置に文字列をこのインスタンスに挿入します。 |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | 指定された文字位置に指定された文字列の 1 つ以上のコピーをこのインスタンスに挿入します。 |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | 指定された文字位置に decimal 数の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, long value)](#insert-int-long-) | 指定された文字位置に long 数の文字列表現をこのインスタンスに挿入します。 |
| [insert(int index, short value)](#insert-int-short-) | 指定された文字位置に short 数の文字列表現をこのインスタンスに挿入します。 |
| [remove(int startIndex, int length)](#remove-int-int-) | このインスタンスから指定された文字範囲を削除します。 |
| [replace(char oldChar, char newChar)](#replace-char-char-) | このインスタンス内の指定された文字のすべての出現を、別の指定された文字に置き換えます。 |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | このインスタンスのサブ文字列内で、指定された文字のすべての出現を別の指定された文字に置き換えます。 |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | このインスタンス内の指定された文字列のすべての出現を、別の指定された文字列に置き換えます。 |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | このインスタンスのサブ文字列内で、指定された文字列のすべての出現を別の指定された文字列に置き換えます。 |
| [setCapacity(int value)](#setCapacity-int-) | 現在のインスタンスが割り当てたメモリに格納できる最大文字数を設定します。 |
| [setLength(int value)](#setLength-int-) | 現在の StringBuilder オブジェクトの長さを設定します。 |
| [toString()](#toString--) | このインスタンスの値を文字列に変換します。 |
| [toString(int startIndex, int length)](#toString-int-int-) | このインスタンスのサブ文字列の値を文字列に変換します。 |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


StringBuilder クラスの新しいインスタンスを初期化します。

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


指定された容量を使用して、StringBuilder クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 容量 | int | このインスタンスの推奨開始サイズです。 |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


指定された容量で開始し、指定された最大値まで拡張できる StringBuilder クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 容量 | int | StringBuilder の推奨開始サイズです。 |
| 最大容量 | int | 現在の文字列が保持できる最大文字数です。 |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


指定された文字列を使用して、StringBuilder クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | インスタンスの値を初期化するために使用される文字列です。 |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


指定された文字列と容量を使用して、StringBuilder クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | インスタンスの値を初期化するために使用される文字列です。 |
| 容量 | int | StringBuilder の推奨開始サイズです。 |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


指定されたサブ文字列と容量から、StringBuilder クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | このインスタンスの値を初期化するために使用されるサブ文字列を含む文字列です。 |
| 開始インデックス | int | サブ文字列が開始する value 内の位置です。 |
| 長さ | int | サブ文字列内の文字数です。 |
| 容量 | int | StringBuilder の推奨開始サイズです。 |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


指定されたブール値の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 追加するブール値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


指定されたバイトの文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | バイト | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


指定された Unicode 文字の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | 文字 | 追加する Unicode 文字です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Unicode 文字の文字列表現の指定された回数分のコピーをこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | 文字 | 追加する文字。 |
| repeatCount | int | 値を追加する回数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


指定された配列内の Unicode 文字の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | char[] | 追加する文字の配列。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


指定された Unicode 文字のサブ配列の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | char[] | 文字配列。 |
| 開始インデックス | int | 値内の開始位置。 |
| charCount | int | 追加する文字数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


指定された double 数値の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


指定された float 数値の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


指定された int 数値の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


指定されたオブジェクトの文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Object | 追加するオブジェクト。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


指定された文字列のコピーをこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加する文字列。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


指定されたサブ文字列のコピーをこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加するサブ文字列を含む文字列。 |
| 開始インデックス | int | 値内のサブ文字列の開始位置。 |
| count | int | 値に追加する文字数。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


指定された BigDecimal 数値の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


指定された long 数の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | long | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


指定された short 数の文字列表現をこのインスタンスに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | short | 追加する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


複合書式文字列（0 個以上の書式項目を含む）を処理して返された文字列をこのインスタンスに追加します。各書式項目は、パラメータ配列内の対応する引数の文字列表現に置き換えられます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| format | java.lang.String | 複合書式文字列。 |
| args | java.lang.Object[] | 書式設定するオブジェクトの配列。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


現在の StringBuilder オブジェクトの末尾にデフォルトの改行文字を追加します。

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


指定された文字列のコピーとデフォルトの改行文字を続けて、現在の StringBuilder オブジェクトの末尾に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加する文字列。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


このインスタンスの指定されたセグメントから文字をコピーし、宛先 Char 配列の指定されたセグメントへ配置します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceIndex | int | このインスタンスで文字がコピーされる開始位置。インデックスはゼロベースです。 |
| destination | char[] | 文字がコピーされる配列です。 |
| destinationIndex | int | 文字がコピーされる destination の開始位置です。インデックスはゼロベースです。 |
| count | int | コピーされる文字数です。 |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


この StringBuilder インスタンスの容量が指定された値以上であることを保証します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 容量 | int | 確保すべき最小容量です。 |

**Returns:**
int - このインスタンスの新しい容量です。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクト、または null です。 |

**Returns:**
boolean - このインスタンスと sb の文字列、Capacity、MaxCapacity の値が等しい場合は true、そうでない場合は false です。
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


現在のインスタンスが割り当てたメモリに格納できる最大文字数を取得します。

**Returns:**
int - 現在のインスタンスが割り当てたメモリに格納できる最大文字数です。
### getLength() {#getLength--}
```
public int getLength()
```


現在の StringBuilder オブジェクトの長さを取得します。

**Returns:**
int - このインスタンスの長さです。
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


このインスタンスの最大容量を取得します。

**Returns:**
int - このインスタンスが保持できる最大文字数です。
### hashCode() {#hashCode--}
```
public int hashCode()
```


この StringBuilder のハッシュコードを返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


指定された文字位置に boolean 値の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | boolean | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


指定された文字位置に byte 値の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | バイト | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


指定された文字位置に指定された Unicode 文字の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | 文字 | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


指定された文字位置に指定された Unicode 文字配列の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | char[] | 挿入する文字配列です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


指定された文字位置に指定された Unicode 文字サブ配列の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | char[] | 文字配列。 |
| 開始インデックス | int | value 内の開始インデックスです。 |
| charCount | int | 挿入する文字数です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


指定された文字位置に double 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | double | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


指定された文字位置に float 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | float | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


指定された文字位置に int 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | int | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


指定された文字位置にオブジェクトの文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | java.lang.Object | 挿入するオブジェクト、または null です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


指定された文字位置に文字列をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | java.lang.String | 挿入する文字列です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


指定された文字位置に指定された文字列の 1 つ以上のコピーをこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | java.lang.String | 挿入する文字列です。 |
| count | int | value を挿入する回数です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


指定された文字位置に decimal 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | java.math.BigDecimal | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


指定された文字位置に long 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | long | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


指定された文字位置に short 数の文字列表現をこのインスタンスに挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 挿入が開始されるこのインスタンス内の位置です。 |
| 値 | short | 挿入する値です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


このインスタンスから指定された文字範囲を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始インデックス | int | 削除が開始されるこのインスタンス内のゼロベース位置です。 |
| 長さ | int | 削除する文字数です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


このインスタンス内の指定された文字のすべての出現を、別の指定された文字に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldChar | 文字 | 置換する文字です。 |
| newChar | 文字 | oldChar を置き換える文字です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


このインスタンスのサブ文字列内で、指定された文字のすべての出現を別の指定された文字に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldValue | 文字 | 置換する文字です。 |
| newValue | 文字 | oldChar を置き換える文字です。 |
| 開始インデックス | int | このインスタンスで部分文字列が開始する位置です。 |
| count | int | 部分文字列の長さです。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


このインスタンス内の指定された文字列のすべての出現を、別の指定された文字列に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldValue | java.lang.String | 置き換える文字列です。 |
| newValue | java.lang.String | oldValue を置き換える文字列、または null です。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


このインスタンスのサブ文字列内で、指定された文字列のすべての出現を別の指定された文字列に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldValue | java.lang.String | 置き換える文字列です。 |
| newValue | java.lang.String | oldValue を置き換える文字列、または null です。 |
| 開始インデックス | int | このインスタンスで部分文字列が開始する位置です。 |
| count | int | 部分文字列の長さです。 |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


現在のインスタンスが割り当てたメモリに格納できる最大文字数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 現在のインスタンスが割り当てたメモリに格納できる最大文字数です。 |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


現在の StringBuilder オブジェクトの長さを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | このインスタンスの長さです。 |

### toString() {#toString--}
```
public String toString()
```


このインスタンスの値を文字列に変換します。

**Returns:**
java.lang.String - このインスタンスと同じ値を持つ文字列です。
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


このインスタンスのサブ文字列の値を文字列に変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始インデックス | int | このインスタンスにおける部分文字列の開始位置です。 |
| 長さ | int | 部分文字列の長さです。 |

**Returns:**
java.lang.String - このインスタンスの指定された部分文字列と同じ値を持つ文字列です。
