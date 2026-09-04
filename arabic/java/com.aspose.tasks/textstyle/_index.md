---
title: "TextStyle"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "غيّر النمط البصري للنص لعنصر في عرض المشروع."
type: docs
weight: 315
url: /ar/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

غيّر النمط البصري للنص لعنصر في عرض المشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TextStyle()](#TextStyle--) | ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالإعدادات الافتراضية. |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالخط الافتراضي وحجم الخط المحدد والنمط. |
| [TextStyle(int fontStyle)](#TextStyle-int-) | ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالخط الافتراضي والنمط المحدد للخط. |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالإعدادات المحددة للخط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل على لون الخلفية لنمط النص. |
| [getBackgroundPattern()](#getBackgroundPattern--) | يحصل على نمط الخلفية لنمط النص. |
| [getColor()](#getColor--) | يحصل على لون النص. |
| [getFont()](#getFont--) | يحصل على الخط لنمط النص. |
| [getItemType()](#getItemType--) | يحصل على [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | يضبط لون الخلفية لنمط النص. |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | يضبط نمط الخلفية لنمط النص. |
| [setColor(Color value)](#setColor-java.awt.Color-) | يضبط لون النص. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | يضبط الخط لنمط النص. |
| [setItemType(int value)](#setItemType-int-) | يضبط [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالإعدادات الافتراضية.

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالخط الافتراضي وحجم الخط المحدد والنمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontSize | float | حجم الخط لنمط النص. |
| fontStyle | int | نمط الخط لنمط النص. |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالخط الافتراضي والنمط المحدد للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontStyle | int | نمط الخط لتطبيقه على الخط الافتراضي. |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


ينشئ نسخة جديدة من فئة [TextStyle](../../com.aspose.tasks/textstyle) بالإعدادات المحددة للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | خط نمط النص. |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


يحصل على لون الخلفية لنمط النص. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - لون الخلفية لنمط النص.
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


يحصل على نمط الخلفية لنمط النص. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - نمط الخلفية لنمط النص.
### getColor() {#getColor--}
```
public final Color getColor()
```


يحصل على لون النص.

**Returns:**
java.awt.Color - لون النص.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


يحصل على الخط لنمط النص.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


يحصل على [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص.

**Returns:**
int - [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص.
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


يضبط لون الخلفية لنمط النص. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الخلفية لنمط النص. |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


يضبط نمط الخلفية لنمط النص. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط الخلفية لنمط النص. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


يضبط لون النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون النص. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


يضبط الخط لنمط النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | خط نمط النص. |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


يضبط [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | [TextItemType](../../com.aspose.tasks/textitemtype) لنمط النص. |

