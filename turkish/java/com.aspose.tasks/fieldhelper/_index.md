---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Alanlarla ilgili faydalı işlemler sağlayan yardımcı sınıf."
type: docs
weight: 88
url: /tr/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Alanlarla ilgili faydalı işlemler sağlayan yardımcı sınıf.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Belirli alanın varsayılan başlığını döndürür. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Belirli görev alanının varsayılan başlığını döndürür. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Belirli alanın varsayılan başlığını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | int | Varsayılan bir başlık almak için alan. |

**Returns:**
java.lang.String - Alan MS Project görünümünde gösterilebiliyorsa belirli alanın varsayılan başlığı, aksi takdirde null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Belirli görev alanının varsayılan başlığını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskKey | byte | Varsayılan bir başlık almak için görev alanı. |

**Returns:**
java.lang.String - Alan MS Project görünümünde gösterilebiliyorsa belirli görev alanının varsayılan başlığı, aksi takdirde null.
