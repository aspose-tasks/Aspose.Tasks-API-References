---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir VBA modülünü temsil eder."
type: docs
weight: 334
url: /tr/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Bir VBA modülünü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | [VbaModule](../../com.aspose.tasks/vbamodule) VbaModuleType.ClassModule türünde bir örnek oluşturur. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | [VbaModule](../../com.aspose.tasks/vbamodule) VbaModuleType.ProceduralModule türünde bir örnek oluşturur. |
| [getAttributes()](#getAttributes--) | Modülün özniteliklerinin bir koleksiyonunu alır. |
| [getName()](#getName--) | VBA modülünün adını alır. |
| [getSourceCode()](#getSourceCode--) | VBA modülünün kaynak kodunu alır. |
| [getType()](#getType--) | Modülün tipini alır. |
| [setName(String value)](#setName-java.lang.String-) | VBA modülünün adı |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | VBA modülünün kaynak kodunu ayarlar. |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


[VbaModule](../../com.aspose.tasks/vbamodule) VbaModuleType.ClassModule türünde bir örnek oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


[VbaModule](../../com.aspose.tasks/vbamodule) VbaModuleType.ProceduralModule türünde bir örnek oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Modülün özniteliklerinin bir koleksiyonunu alır.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


VBA modülünün adını alır.

**Returns:**
java.lang.String - VBA modülünün adı
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


VBA modülünün kaynak kodunu alır.

**Returns:**
java.lang.String - VBA modülünün kaynak kodu
### getType() {#getType--}
```
public final int getType()
```


Modülün tipini alır.

**Returns:**
int - modülün tipi.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


VBA modülünün adı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | VBA modülünün adı |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


VBA modülünün kaynak kodunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | VBA modülünün kaynak kodu |

