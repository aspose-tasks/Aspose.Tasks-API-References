---
title: "VbaModule"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक VBA मॉड्यूल को दर्शाता है।"
type: docs
weight: 334
url: /hi/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

एक VBA मॉड्यूल को दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | VbaModuleType.ClassModule प्रकार के साथ [VbaModule](../../com.aspose/tasks/vbamodule) का एक उदाहरण बनाता है। |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | VbaModuleType.ProceduralModule प्रकार के साथ [VbaModule](../../com.aspose/tasks/vbamodule) का एक उदाहरण बनाता है। |
| [getAttributes()](#getAttributes--) | मॉड्यूल के गुणों का संग्रह प्राप्त करता है। |
| [getName()](#getName--) | VBA मॉड्यूल का नाम प्राप्त करता है |
| [getSourceCode()](#getSourceCode--) | VBA मॉड्यूल का स्रोत कोड प्राप्त करता है |
| [getType()](#getType--) | मॉड्यूल का प्रकार प्राप्त करता है। |
| [setName(String value)](#setName-java.lang.String-) | VBA मॉड्यूल का नाम |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | VBA मॉड्यूल का स्रोत कोड सेट करता है |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


VbaModuleType.ClassModule प्रकार के साथ [VbaModule](../../com.aspose/tasks/vbamodule) का एक उदाहरण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


VbaModuleType.ProceduralModule प्रकार के साथ [VbaModule](../../com.aspose/tasks/vbamodule) का एक उदाहरण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


मॉड्यूल के गुणों का संग्रह प्राप्त करता है।

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


VBA मॉड्यूल का नाम प्राप्त करता है

**Returns:**
java.lang.String - VBA मॉड्यूल का नाम
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


VBA मॉड्यूल का स्रोत कोड प्राप्त करता है

**Returns:**
java.lang.String - VBA मॉड्यूल का स्रोत कोड
### getType() {#getType--}
```
public final int getType()
```


मॉड्यूल का प्रकार प्राप्त करता है।

**Returns:**
int - मॉड्यूल का प्रकार।
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


VBA मॉड्यूल का नाम

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | VBA मॉड्यूल का नाम |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


VBA मॉड्यूल का स्रोत कोड सेट करता है

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | VBA मॉड्यूल का स्रोत कोड |

