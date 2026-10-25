---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Değiştirilebilir bir karakter dizisini temsil eder."
type: docs
weight: 281
url: /tr/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Değiştirilebilir bir karakter dizisini temsil eder. Uzatılamaz.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | StringBuilder sınıfının yeni bir örneğini başlatır. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Belirtilen kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Belirtilen bir kapasiteyle başlayan ve belirtilen bir maksimuma kadar büyüyebilen StringBuilder sınıfının yeni bir örneğini başlatır. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Belirtilen dizeyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Belirtilen dizeyi ve kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Belirtilen alt dizeyi ve kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Belirtilen bir boolean değerinin dize temsilini bu örneğe ekler. |
| [append(byte value)](#append-byte-) | Belirtilen bir baytın dize temsilini bu örneğe ekler. |
| [append(char value)](#append-char-) | Belirtilen bir Unicode karakterinin dize temsilini bu örneğe ekler. |
| [append(char value, int repeatCount)](#append-char-int-) | Unicode karakterinin dize temsilinin belirtilen sayıda kopyasını bu örneğe ekler. |
| [append(char[] value)](#append-char---) | Belirtilen bir dizideki Unicode karakterlerinin dize temsilini bu örneğe ekler. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Belirtilen bir Unicode karakter alt dizisinin dize temsilini bu örneğe ekler. |
| [append(double value)](#append-double-) | Belirtilen bir double sayısının dize temsilini bu örneğe ekler. |
| [append(float value)](#append-float-) | Belirtilen bir float sayısının dize temsilini bu örneğe ekler. |
| [append(int value)](#append-int-) | Belirtilen bir int sayısının dize temsilini bu örneğe ekler. |
| [append(Object value)](#append-java.lang.Object-) | Belirtilen bir nesnenin dize temsilini bu örneğe ekler. |
| [append(String value)](#append-java.lang.String-) | Belirtilen dizeyi bir kopyasını bu örneğe ekler. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Belirtilen bir alt dizeyi bir kopyasını bu örneğe ekler. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Belirtilen bir BigDecimal sayısının dize temsilini bu örneğe ekler. |
| [append(long value)](#append-long-) | Belirtilen uzun sayının dize temsilini bu örneğe ekler. |
| [append(short value)](#append-short-) | Belirtilen kısa sayının dize temsilini bu örneğe ekler. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Bir veya daha fazla biçim öğesi içeren birleşik biçim dizesini işleyerek döndürülen dizeyi bu örneğe ekler. |
| [appendLine()](#appendLine--) | Geçerli StringBuilder nesnesinin sonuna varsayılan satır sonlandırıcısını ekler. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Belirtilen dizeyi, ardından varsayılan satır sonlandırıcısını ekleyerek, geçerli StringBuilder nesnesinin sonuna ekler. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Bu örneğin belirtilen bir segmentindeki karakterleri, hedef Char dizisinin belirtilen bir segmentine kopyalar. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Bu StringBuilder örneğinin kapasitesinin en az belirtilen değer olmasını sağlar. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getCapacity()](#getCapacity--) | Geçerli örnek tarafından tahsis edilen bellekte bulunabilecek azami karakter sayısını alır. |
| [getLength()](#getLength--) | Geçerli StringBuilder nesnesinin uzunluğunu alır. |
| [getMaxCapacity()](#getMaxCapacity--) | Bu örneğin azami kapasitesini alır. |
| [hashCode()](#hashCode--) | Bu StringBuilder için bir karma kodu döndürür. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Belirtilen karakter konumunda bu örneğe bir boolean değerinin dize temsilini ekler. |
| [insert(int index, byte value)](#insert-int-byte-) | Belirtilen karakter konumunda bu örneğe bir byte değerinin dize temsilini ekler. |
| [insert(int index, char value)](#insert-int-char-) | Belirtilen karakter konumunda bu örneğe belirtilen bir Unicode karakterinin dize temsilini ekler. |
| [insert(int index, char[] value)](#insert-int-char---) | Belirtilen karakter konumunda bu örneğe belirtilen Unicode karakter dizisinin dize temsilini ekler. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Belirtilen karakter konumunda bu örneğe belirtilen Unicode karakter alt dizisinin dize temsilini ekler. |
| [insert(int index, double value)](#insert-int-double-) | Belirtilen karakter konumunda bu örneğe bir double sayının dize temsilini ekler. |
| [insert(int index, float value)](#insert-int-float-) | Belirtilen karakter konumunda bu örneğe bir float sayının dize temsilini ekler. |
| [insert(int index, int value)](#insert-int-int-) | Belirtilen karakter konumunda bu örneğe bir int sayının dize temsilini ekler. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Belirtilen karakter konumunda bu örneğe bir nesnenin dize temsilini ekler. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Belirtilen karakter konumunda bu örneğe bir dize ekler. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Belirtilen karakter konumunda bu örneğe belirtilen bir dizeyi bir veya daha fazla kopya olarak ekler. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Belirtilen karakter konumunda bu örneğe bir decimal sayının dize temsilini ekler. |
| [insert(int index, long value)](#insert-int-long-) | Belirtilen karakter konumunda bu örneğe bir long sayının dize temsilini ekler. |
| [insert(int index, short value)](#insert-int-short-) | Belirtilen karakter konumunda bu örneğe bir short sayının dize temsilini ekler. |
| [remove(int startIndex, int length)](#remove-int-int-) | Bu örnekten belirtilen karakter aralığını kaldırır. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Bu örnekte belirtilen bir karakterin tüm görünümlerini başka bir belirtilen karakterle değiştirir. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Bu örneğin bir alt dizesi içinde, belirtilen bir karakterin tüm görünümlerini başka bir belirtilen karakterle değiştirir. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Bu örnekte belirtilen bir dizenin tüm görünümlerini başka bir belirtilen dizeyle değiştirir. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Bu örneğin bir alt dizesi içinde, belirtilen bir dizenin tüm görünümlerini başka bir belirtilen dizeyle değiştirir. |
| [setCapacity(int value)](#setCapacity-int-) | Geçerli örnek tarafından ayrılan bellekte bulunabilecek maksimum karakter sayısını ayarlar. |
| [setLength(int value)](#setLength-int-) | Geçerli StringBuilder nesnesinin uzunluğunu ayarlar. |
| [toString()](#toString--) | Bu örneğin değerini bir String'e dönüştürür. |
| [toString(int startIndex, int length)](#toString-int-int-) | Bu örneğin bir alt dizesinin değerini bir String'e dönüştürür. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


StringBuilder sınıfının yeni bir örneğini başlatır.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Belirtilen kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kapasite | int | Bu örnek için önerilen başlangıç boyutu. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Belirtilen bir kapasiteyle başlayan ve belirtilen bir maksimuma kadar büyüyebilen StringBuilder sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kapasite | int | StringBuilder için önerilen başlangıç boyutu. |
| maxCapacity | int | Geçerli dizenin içerebileceği maksimum karakter sayısı. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Belirtilen dizeyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Örneğin değerini başlatmak için kullanılan dize. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Belirtilen dizeyi ve kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Örneğin değerini başlatmak için kullanılan dize. |
| kapasite | int | StringBuilder için önerilen başlangıç boyutu. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Belirtilen alt dizeyi ve kapasiteyi kullanarak StringBuilder sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Bu örneğin değerini başlatmak için kullanılan alt dizeyi içeren dize. |
| startIndex | int | Alt dizenin başladığı değerdeki konum. |
| length | int | Alt dizedeki karakter sayısı. |
| kapasite | int | StringBuilder için önerilen başlangıç boyutu. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Belirtilen bir boolean değerinin dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Eklenecek boolean değeri. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Belirtilen bir baytın dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Belirtilen bir Unicode karakterinin dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char | Eklenecek Unicode karakteri. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Unicode karakterinin dize temsilinin belirtilen sayıda kopyasını bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char | Eklenecek karakter. |
| repeatCount | int | Değeri ekleme sayısı. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Belirtilen bir dizideki Unicode karakterlerinin dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char[] | Eklenecek karakter dizisi. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Belirtilen bir Unicode karakter alt dizisinin dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char[] | Bir karakter dizisi. |
| startIndex | int | Değer içindeki başlangıç konumu. |
| charCount | int | Eklenecek karakter sayısı. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Belirtilen bir double sayısının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Belirtilen bir float sayısının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Belirtilen bir int sayısının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Belirtilen bir nesnenin dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Eklenecek nesne. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Belirtilen dizeyi bir kopyasını bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenecek dize. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Belirtilen bir alt dizeyi bir kopyasını bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Alt dizeyi içeren eklenecek dize. |
| startIndex | int | Değer içindeki alt dizenin başlangıç konumu. |
| count | int | Değer içinde eklenecek karakter sayısı. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Belirtilen bir BigDecimal sayısının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Belirtilen uzun sayının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | long | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Belirtilen kısa sayının dize temsilini bu örneğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Bir birleşik biçim dizesini işleyerek döndürülen dizeyi bu örneğe ekler; bu dize sıfır veya daha fazla biçim öğesi içerir. Her biçim öğesi, parametre dizisindeki ilgili argümanın dize temsilcisiyle değiştirilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | java.lang.String | Bir birleşik biçim dizesi. |
| args | java.lang.Object[] | Biçimlendirilecek nesneler dizisi. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Geçerli StringBuilder nesnesinin sonuna varsayılan satır sonlandırıcısını ekler.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Belirtilen dizeyi, ardından varsayılan satır sonlandırıcısını ekleyerek, geçerli StringBuilder nesnesinin sonuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenecek dize. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Bu örneğin belirtilen bir segmentindeki karakterleri, hedef Char dizisinin belirtilen bir segmentine kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | int | Bu örnekte karakterlerin kopyalanacağı başlangıç konumu. İndeks sıfır tabanlıdır. |
| hedef | char[] | Karakterlerin kopyalanacağı dizi. |
| hedefIndeksi | int | Karakterlerin kopyalanacağı hedefteki başlangıç konumu. İndeks sıfır tabanlıdır. |
| count | int | Kopyalanacak karakter sayısı. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Bu StringBuilder örneğinin kapasitesinin en az belirtilen değer olmasını sağlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kapasite | int | Garantilenmesi gereken minimum kapasite. |

**Returns:**
int - Bu örneğin yeni kapasitesi.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak bir nesne veya null. |

**Returns:**
boolean - bu örnek ve sb eşit string, Capacity ve MaxCapacity değerlerine sahipse true; aksi takdirde false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Geçerli örnek tarafından tahsis edilen bellekte bulunabilecek azami karakter sayısını alır.

**Returns:**
int - mevcut örnek tarafından ayrılan bellekte bulunabilecek maksimum karakter sayısı.
### getLength() {#getLength--}
```
public int getLength()
```


Geçerli StringBuilder nesnesinin uzunluğunu alır.

**Returns:**
int - Bu örneğin uzunluğu.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Bu örneğin azami kapasitesini alır.

**Returns:**
int - Bu örneğin tutabileceği maksimum karakter sayısı.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bu StringBuilder için bir karma kodu döndürür.

**Returns:**
int - Bu nesne için bir karma kod değeri döndürür.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Belirtilen karakter konumunda bu örneğe bir boolean değerinin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | boolean | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Belirtilen karakter konumunda bu örneğe bir byte değerinin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | byte | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Belirtilen karakter konumunda bu örneğe belirtilen bir Unicode karakterinin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | char | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Belirtilen karakter konumunda bu örneğe belirtilen Unicode karakter dizisinin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | char[] | Eklenecek karakter dizisi. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Belirtilen karakter konumunda bu örneğe belirtilen Unicode karakter alt dizisinin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | char[] | Bir karakter dizisi. |
| startIndex | int | Değer içindeki başlangıç indeksi. |
| charCount | int | Eklenecek karakter sayısı. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Belirtilen karakter konumunda bu örneğe bir double sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | double | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Belirtilen karakter konumunda bu örneğe bir float sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | float | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Belirtilen karakter konumunda bu örneğe bir int sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | int | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Belirtilen karakter konumunda bu örneğe bir nesnenin dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | java.lang.Object | Eklenecek nesne veya null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Belirtilen karakter konumunda bu örneğe bir dize ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | java.lang.String | Eklenecek dize. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Belirtilen karakter konumunda bu örneğe belirtilen bir dizeyi bir veya daha fazla kopya olarak ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | java.lang.String | Eklenecek dize. |
| count | int | Değerin kaç kez ekleneceği. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Belirtilen karakter konumunda bu örneğe bir decimal sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | java.math.BigDecimal | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Belirtilen karakter konumunda bu örneğe bir long sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | long | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Belirtilen karakter konumunda bu örneğe bir short sayının dize temsilini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Eklemenin başladığı bu örnekteki konum. |
| değer | short | Eklenecek değer. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Bu örnekten belirtilen karakter aralığını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Kaldırmanın başladığı bu örnekteki sıfır tabanlı konum. |
| length | int | Kaldırılacak karakter sayısı. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Bu örnekte belirtilen bir karakterin tüm görünümlerini başka bir belirtilen karakterle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| eskiKarakter | char | Değiştirilecek karakter. |
| yeniKarakter | char | oldChar karakterini değiştiren karakter. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Bu örneğin bir alt dizesi içinde, belirtilen bir karakterin tüm görünümlerini başka bir belirtilen karakterle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | char | Değiştirilecek karakter. |
| newValue | char | oldChar karakterini değiştiren karakter. |
| startIndex | int | Bu örnekte alt dizenin başladığı konum. |
| count | int | Alt dizenin uzunluğu. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Bu örnekte belirtilen bir dizenin tüm görünümlerini başka bir belirtilen dizeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | java.lang.String | Değiştirilecek dize. |
| newValue | java.lang.String | oldValue değerini değiştiren dize ya da null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Bu örneğin bir alt dizesi içinde, belirtilen bir dizenin tüm görünümlerini başka bir belirtilen dizeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | java.lang.String | Değiştirilecek dize. |
| newValue | java.lang.String | oldValue değerini değiştiren dize ya da null. |
| startIndex | int | Bu örnekte alt dizenin başladığı konum. |
| count | int | Alt dizenin uzunluğu. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Geçerli örnek tarafından ayrılan bellekte bulunabilecek maksimum karakter sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Mevcut örnek tarafından ayrılan bellekte bulunabilecek azami karakter sayısı. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Geçerli StringBuilder nesnesinin uzunluğunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Bu örneğin uzunluğu. |

### toString() {#toString--}
```
public String toString()
```


Bu örneğin değerini bir String'e dönüştürür.

**Returns:**
java.lang.String - Bu örnek ile aynı değere sahip bir dize.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Bu örneğin bir alt dizesinin değerini bir String'e dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Bu örnekte alt dizenin başlangıç konumu. |
| length | int | Alt dizenin uzunluğu. |

**Returns:**
java.lang.String - Bu örneğin belirtilen alt dizesiyle aynı değere sahip bir dize.
