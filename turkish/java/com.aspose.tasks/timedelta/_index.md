---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API Referansı"
description: "İki zaman damgası arasındaki farkı temsil eder."
type: docs
weight: 317
url: /tr/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

İki zaman damgası arasındaki farkı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | TimeDelta'ın yeni örneğini belirtilen saat, dakika ve saniye sayısına başlatır. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | TimeDelta'ın yeni örneğini belirtilen gün, saat, dakika, saniye ve milisaniye sayısına başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Bu ve diğer örneklerin toplamı olan yeni bir TimeDelta nesnesini döndürür. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | İki TimeDelta değerini karşılaştırır ve ilk değerin ikinci değerden daha kısa, eşit veya daha uzun olduğunu belirten bir tamsayı döndürür. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Bu örneği belirtilen bir TimeDelta nesnesiyle karşılaştırır ve bu örneğin TimeSpan nesnesinden daha kısa, eşit veya daha uzun olduğunu belirten bir tamsayı döndürür. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | `other` zaman aralığının bu ile eşit olup olmadığını gösterir. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | İki örneğin eşitliğini kontrol eder. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Belirtilen gün sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır). |
| [fromHours(double value)](#fromHours-double-) | Belirtilen saat sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Belirtilen milisaniye sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır). |
| [fromMinutes(double value)](#fromMinutes-double-) | Belirtilen dakika sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır). |
| [fromSeconds(double value)](#fromSeconds-double-) | Belirtilen saniye sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır). |
| [getDays()](#getDays--) | Bu örnek tarafından temsil edilen zaman aralığının gün bileşenini döndürür. |
| [getHours()](#getHours--) | Bu örnek tarafından temsil edilen zaman aralığının saat bileşenini döndürür. |
| [getMilliseconds()](#getMilliseconds--) | Bu örnek tarafından temsil edilen zaman aralığının milisaniye bileşenini döndürür. |
| [getMinutes()](#getMinutes--) | Bu örnek tarafından temsil edilen zaman aralığının dakika bileşenini döndürür. |
| [getSeconds()](#getSeconds--) | Bu örnek tarafından temsil edilen zaman aralığının saniye bileşenini döndürür. |
| [getTotalDays()](#getTotalDays--) | Mevcut örneğin değerini tam ve kesirli gün cinsinden döndürür. |
| [getTotalHours()](#getTotalHours--) | Mevcut örneğin değerini tam ve kesirli saat cinsinden döndürür. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Mevcut örneğin değerini tam ve kesirli milisaniye cinsinden döndürür. |
| [getTotalMinutes()](#getTotalMinutes--) | Mevcut örneğin değerini tam ve kesirli dakika cinsinden döndürür. |
| [getTotalSeconds()](#getTotalSeconds--) | Mevcut örneğin değerini tam ve kesirli saniye cinsinden döndürür. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Bu örneğin değerinin negatifine sahip yeni bir `TimeDelta` döndürür. |
| [parse(String s)](#parse-java.lang.String-) | Bir zaman aralığının dize temsilini `TimeDelta` eşdeğerine dönüştürür. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Bu ve `other` örnekleri arasındaki farkı değer olarak taşıyan yeni bir TimeDelta nesnesi döndürür. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Bir zaman aralığının dize temsilini TimeDelta eşdeğerine dönüştürür ve dönüşümün başarılı olup olmadığını gösteren bir değer döndürür. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


TimeDelta'ın yeni örneğini belirtilen saat, dakika ve saniye sayısına başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saat | int | saat sayısı. |
| dakika | int | dakika sayısı. |
| saniyeler | int | saniye sayısı. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


TimeDelta'ın yeni örneğini belirtilen gün, saat, dakika, saniye ve milisaniye sayısına başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gün | int | gün sayısı. |
| saat | int | saat sayısı. |
| dakika | int | dakika sayısı. |
| saniyeler | int | saniye sayısı. |
| milisaniye | int | milisaniye sayısı. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Bu ve diğer örneklerin toplamı olan yeni bir TimeDelta nesnesini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | toplamak için örnek. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


İki TimeDelta değerini karşılaştırır ve ilk değerin ikinci değerden daha kısa, eşit veya daha uzun olduğunu belirten bir tamsayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | karşılaştırılacak ilk zaman aralığı. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | karşılaştırılacak ikinci zaman aralığı. |

**Returns:**
int - \-1 eğer `t1` `t2`'den daha kısa ise, 0 eğer `t1` `t2`'ye eşitse ve 1 eğer `t1` `t2`'den daha uzun ise.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Bu örneği belirtilen bir TimeDelta nesnesiyle karşılaştırır ve bu örneğin TimeSpan nesnesinden daha kısa, eşit veya daha uzun olduğunu belirten bir tamsayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | karşılaştırılacak bir örnek. |

**Returns:**
int - \-1 eğer bu örnek `other`'dan daha kısa ise, 0 eğer bu örnek `other`'a eşitse ve 1 eğer bu örnek `other`'dan daha uzun ise.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


`other` zaman aralığının bu ile eşit olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | karşılaştırılacak zaman aralığı. |

**Returns:**
boolean - aralıklar eşitse `true`; aksi takdirde `false`.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


İki örneğin eşitliğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | ilk örnek. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | ikinci örnek. |

**Returns:**
boolean - örnekler eşitse `true`; aksi takdirde `false`.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Belirtilen gün sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir gün sayısı. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Belirtilen saat sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir saat sayısı. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Belirtilen milisaniye sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir milisaniye sayısı. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Belirtilen dakika sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir dakika sayısı. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Belirtilen saniye sayısını temsil eden bir TimeDelta döndürür (en yakın milisaniyeye yuvarlanır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir saniye sayısı. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Bu örnek tarafından temsil edilen zaman aralığının gün bileşenini döndürür.

**Returns:**
int - zaman aralığının gün bileşeni. Pozitif ya da negatif olabilir.
### getHours() {#getHours--}
```
public int getHours()
```


Bu örnek tarafından temsil edilen zaman aralığının saat bileşenini döndürür.

**Returns:**
int - zaman aralığının saat bileşeni, -23 ile 23 arasında.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Bu örnek tarafından temsil edilen zaman aralığının milisaniye bileşenini döndürür.

**Returns:**
int - zaman aralığının milisaniye bileşeni, -999 ile 999 arasında.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Bu örnek tarafından temsil edilen zaman aralığının dakika bileşenini döndürür.

**Returns:**
int - zaman aralığının -59 ile 59 arasındaki dakikalar bileşeni.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Bu örnek tarafından temsil edilen zaman aralığının saniye bileşenini döndürür.

**Returns:**
int - zaman aralığının -59 ile 59 arasındaki saniyeler bileşeni.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Mevcut örneğin değerini tam ve kesirli gün cinsinden döndürür.

**Returns:**
double - bu örnek tarafından temsil edilen toplam gün sayısı.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Mevcut örneğin değerini tam ve kesirli saat cinsinden döndürür.

**Returns:**
double - bu örnek tarafından temsil edilen toplam saat sayısı.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Mevcut örneğin değerini tam ve kesirli milisaniye cinsinden döndürür.

**Returns:**
double - bu örnek tarafından temsil edilen toplam milisaniye sayısı.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Mevcut örneğin değerini tam ve kesirli dakika cinsinden döndürür.

**Returns:**
double - bu örnek tarafından temsil edilen toplam dakika sayısı.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Mevcut örneğin değerini tam ve kesirli saniye cinsinden döndürür.

**Returns:**
double - bu örnek tarafından temsil edilen toplam saniye sayısı.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Bu örneğin değerinin negatifine sahip yeni bir `TimeDelta` döndürür.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Bir zaman aralığının dize temsilini `TimeDelta` eşdeğerine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.lang.String | dönüştürülecek zaman aralığını belirten bir dize. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Bu ve `other` örnekleri arasındaki farkı değer olarak taşıyan yeni bir TimeDelta nesnesi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | çıkarılacak örnek. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Bir zaman aralığının dize temsilini TimeDelta eşdeğerine dönüştürür ve dönüşümün başarılı olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.lang.String | dönüştürülecek zaman aralığını belirten bir dize. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | bu dizi en az bir öğe içermelidir. Bu yöntem döndüğünde, `result[0]` `s` tarafından belirtilen zaman aralığını temsil eden bir nesne içerir veya dönüşüm başarısız olursa sıfır uzunlukta bir zaman aralığı olur. |

**Returns:**
boolean - `true` eğer s başarıyla dönüştürüldüyse; aksi takdirde `false`.
