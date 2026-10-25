---
title: "TimeDelta"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili perbedaan antara dua cap waktu."
type: docs
weight: 317
url: /id/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Mewakili perbedaan antara dua cap waktu.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Menginisialisasi instance baru TimeDelta dengan jumlah jam, menit, dan detik yang ditentukan. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Menginisialisasi instance baru TimeDelta dengan jumlah hari, jam, menit, detik, dan milidetik yang ditentukan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Mengembalikan objek TimeDelta baru yang nilainya merupakan jumlah dari instance ini dan yang lain. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Membandingkan dua nilai TimeDelta dan mengembalikan integer yang menunjukkan apakah nilai pertama lebih pendek, sama, atau lebih panjang daripada nilai kedua. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Membandingkan instance ini dengan objek TimeDelta yang ditentukan dan mengembalikan integer yang menunjukkan apakah instance ini lebih pendek, sama, atau lebih panjang daripada objek TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Menunjukkan apakah beberapa rentang waktu `other` sama dengan yang ini. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Memeriksa dua instance untuk kesetaraan. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Mengembalikan TimeDelta yang mewakili sejumlah hari yang ditentukan (dibulatkan ke milidetik terdekat). |
| [fromHours(double value)](#fromHours-double-) | Mengembalikan TimeDelta yang mewakili sejumlah jam yang ditentukan (dibulatkan ke milidetik terdekat). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Mengembalikan TimeDelta yang mewakili sejumlah milidetik yang ditentukan (dibulatkan ke milidetik terdekat). |
| [fromMinutes(double value)](#fromMinutes-double-) | Mengembalikan TimeDelta yang mewakili sejumlah menit yang ditentukan (dibulatkan ke milidetik terdekat). |
| [fromSeconds(double value)](#fromSeconds-double-) | Mengembalikan TimeDelta yang mewakili sejumlah detik yang ditentukan (dibulatkan ke milidetik terdekat). |
| [getDays()](#getDays--) | Mengembalikan komponen hari dari interval waktu, yang diwakili oleh instance ini. |
| [getHours()](#getHours--) | Mengembalikan komponen jam dari interval waktu, yang diwakili oleh instance ini. |
| [getMilliseconds()](#getMilliseconds--) | Mengembalikan komponen milidetik dari interval waktu, yang diwakili oleh instance ini. |
| [getMinutes()](#getMinutes--) | Mengembalikan komponen menit dari interval waktu, yang diwakili oleh instance ini. |
| [getSeconds()](#getSeconds--) | Mengembalikan komponen detik dari interval waktu, yang diwakili oleh instance ini. |
| [getTotalDays()](#getTotalDays--) | Mengembalikan nilai instance saat ini yang diekspresikan dalam hari penuh dan pecahan. |
| [getTotalHours()](#getTotalHours--) | Mengembalikan nilai instance saat ini yang diekspresikan dalam jam penuh dan pecahan. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Mengembalikan nilai instance saat ini yang diekspresikan dalam milidetik penuh dan pecahan. |
| [getTotalMinutes()](#getTotalMinutes--) | Mengembalikan nilai instance saat ini yang diekspresikan dalam menit penuh dan pecahan. |
| [getTotalSeconds()](#getTotalSeconds--) | Mengembalikan nilai instance saat ini yang diekspresikan dalam detik penuh dan pecahan. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Mengembalikan `TimeDelta` baru yang nilainya merupakan nilai negatif dari instance ini. |
| [parse(String s)](#parse-java.lang.String-) | Mengonversi representasi string dari interval waktu menjadi ekivalen `TimeDelta`-nya. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Mengembalikan objek TimeDelta baru yang nilainya merupakan selisih antara instance ini dan `other`. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Mengonversi representasi string dari interval waktu menjadi ekivalen TimeDelta dan mengembalikan nilai yang menunjukkan apakah konversi berhasil. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Menginisialisasi instance baru TimeDelta dengan jumlah jam, menit, dan detik yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| jam | int | jumlah jam. |
| menit | int | jumlah menit. |
| detik | int | jumlah detik. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Menginisialisasi instance baru TimeDelta dengan jumlah hari, jam, menit, detik, dan milidetik yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| hari | int | jumlah hari. |
| jam | int | jumlah jam. |
| menit | int | jumlah menit. |
| detik | int | jumlah detik. |
| milidetik | int | jumlah milidetik. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Mengembalikan objek TimeDelta baru yang nilainya merupakan jumlah dari instance ini dan yang lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | instansi untuk dijumlahkan dengan. |

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


Membandingkan dua nilai TimeDelta dan mengembalikan integer yang menunjukkan apakah nilai pertama lebih pendek, sama, atau lebih panjang daripada nilai kedua.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | interval waktu pertama untuk dibandingkan. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | interval waktu kedua untuk dibandingkan. |

**Returns:**
int - \-1 jika `t1` lebih pendek dari `t2`, 0 jika `t1` sama dengan `t2` dan 1 jika `t1` lebih panjang dari `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Membandingkan instance ini dengan objek TimeDelta yang ditentukan dan mengembalikan integer yang menunjukkan apakah instance ini lebih pendek, sama, atau lebih panjang daripada objek TimeSpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | sebuah instansi untuk dibandingkan dengan. |

**Returns:**
int - \-1 jika instansi ini lebih pendek dari `other`, 0 jika instansi ini sama dengan `other` dan 1 jika instansi ini lebih panjang dari `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Menunjukkan apakah beberapa rentang waktu `other` sama dengan yang ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | rentang waktu untuk dibandingkan dengan. |

**Returns:**
boolean - `true` jika interval sama; `false` sebaliknya.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Memeriksa dua instance untuk kesetaraan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | instansi pertama. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | instansi kedua. |

**Returns:**
boolean - `true` jika instansi sama; `false` sebaliknya.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lainnya | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Mengembalikan TimeDelta yang mewakili sejumlah hari yang ditentukan (dibulatkan ke milidetik terdekat).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | sejumlah hari. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Mengembalikan TimeDelta yang mewakili sejumlah jam yang ditentukan (dibulatkan ke milidetik terdekat).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | sejumlah jam. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Mengembalikan TimeDelta yang mewakili sejumlah milidetik yang ditentukan (dibulatkan ke milidetik terdekat).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | sejumlah milidetik. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Mengembalikan TimeDelta yang mewakili sejumlah menit yang ditentukan (dibulatkan ke milidetik terdekat).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | sejumlah menit. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Mengembalikan TimeDelta yang mewakili sejumlah detik yang ditentukan (dibulatkan ke milidetik terdekat).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | sejumlah detik. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Mengembalikan komponen hari dari interval waktu, yang diwakili oleh instance ini.

**Returns:**
int - komponen hari dari interval waktu. Dapat bernilai positif atau negatif.
### getHours() {#getHours--}
```
public int getHours()
```


Mengembalikan komponen jam dari interval waktu, yang diwakili oleh instance ini.

**Returns:**
int - komponen jam dari interval waktu dalam rentang -23 hingga 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Mengembalikan komponen milidetik dari interval waktu, yang diwakili oleh instance ini.

**Returns:**
int - komponen milidetik dari interval waktu dalam rentang -999 hingga 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Mengembalikan komponen menit dari interval waktu, yang diwakili oleh instance ini.

**Returns:**
int - komponen menit dari interval waktu dalam rentang -59 hingga 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Mengembalikan komponen detik dari interval waktu, yang diwakili oleh instance ini.

**Returns:**
int - komponen detik dari interval waktu dalam rentang -59 hingga 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Mengembalikan nilai instance saat ini yang diekspresikan dalam hari penuh dan pecahan.

**Returns:**
double - total jumlah hari yang diwakili oleh instance ini.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Mengembalikan nilai instance saat ini yang diekspresikan dalam jam penuh dan pecahan.

**Returns:**
double - total jumlah jam yang diwakili oleh instance ini.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Mengembalikan nilai instance saat ini yang diekspresikan dalam milidetik penuh dan pecahan.

**Returns:**
double - total jumlah milidetik yang diwakili oleh instance ini.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Mengembalikan nilai instance saat ini yang diekspresikan dalam menit penuh dan pecahan.

**Returns:**
double - total jumlah menit yang diwakili oleh instance ini.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Mengembalikan nilai instance saat ini yang diekspresikan dalam detik penuh dan pecahan.

**Returns:**
double - total jumlah detik yang diwakili oleh instance ini.
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


Mengembalikan `TimeDelta` baru yang nilainya merupakan nilai negatif dari instance ini.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Mengonversi representasi string dari interval waktu menjadi ekivalen `TimeDelta`-nya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| s | java.lang.String | string yang menentukan interval waktu yang akan dikonversi. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Mengembalikan objek TimeDelta baru yang nilainya merupakan selisih antara instance ini dan `other`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | instance yang akan dikurangkan. |

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


Mengonversi representasi string dari interval waktu menjadi ekivalen TimeDelta dan mengembalikan nilai yang menunjukkan apakah konversi berhasil.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| s | java.lang.String | string yang menentukan interval waktu yang akan dikonversi. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | array ini harus memiliki setidaknya satu elemen. Ketika metode ini mengembalikan, `result[0]` berisi objek yang mewakili interval waktu yang ditentukan oleh `s`, atau interval waktu dengan panjang nol jika konversi gagal. |

**Returns:**
boolean - `true` jika s berhasil dikonversi; jika tidak, `false`.
