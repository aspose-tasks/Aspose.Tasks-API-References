---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir taslak kodunun değerini temsil eder."
type: docs
weight: 167
url: /tr/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Bir taslak kodunun değerini temsil eder.

--------------------

İki veri parçası gereklidir - FieldId tarafından belirtilen outline kod tablosuna bir işaretçi ve ValueId ya da ValueGuid işaretçisiyle belirtilen değer listesine işaret eden değer.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Yeni bir [OutlineCode](../../com.aspose.tasks/outlinecode) sınıfı örneği başlatır. |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Belirtilen Outline Code ve onun değerlerinden birini kullanarak yeni bir [OutlineCode](../../com.aspose.tasks/outlinecode) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFieldId()](#getFieldId--) | Proje Id özel alanının sayı değerini alır. |
| [getValueGuid()](#getValueGuid--) | Değer listesindeki değerin GUID'ini alır. |
| [getValueId()](#getValueId--) | Outline kod koleksiyonundaki tanımlamayla ilişkili değer listesindeki Id'yi alır. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Proje Id özel alanının sayı değerini ayarlar. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Değer listesindeki değerin GUID'ini ayarlar. |
| [setValueId(int value)](#setValueId-int-) | Outline kod koleksiyonundaki tanımlamayla ilişkili değer listesindeki Id'yi ayarlar. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Yeni bir [OutlineCode](../../com.aspose.tasks/outlinecode) sınıfı örneği başlatır.

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Belirtilen Outline Code ve onun değerlerinden birini kullanarak yeni bir [OutlineCode](../../com.aspose.tasks/outlinecode) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | çizelge kodu tanımı. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | çizelge kodu tanımı değerlerinden biri. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Proje Id özel alanının sayı değerini alır.

**Returns:**
java.lang.String - projenin Id özel alanının sayısal değeri.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Değer listesindeki değerin GUID'ini alır. ValueGuid, değer listesindeki FieldGuid ile eşleşir.

**Returns:**
java.lang.String - değer listesindeki değerin GUID'i.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Outline kod koleksiyonundaki tanımlamayla ilişkili değer listesindeki Id'yi alır.

**Returns:**
int - çizelge kodu koleksiyonundaki tanımla ilişkili değer listesindeki Id.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Proje Id özel alanının sayı değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | projenin Id özel alanının sayısal değeri. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Değer listesindeki değerin GUID'ini ayarlar. ValueGuid, değer listesindeki FieldGuid ile eşleşir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | değer listesindeki değerin GUID'i. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Outline kod koleksiyonundaki tanımlamayla ilişkili değer listesindeki Id'yi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çizelge kodu koleksiyonundaki tanımla ilişkili değer listesindeki Id. |

