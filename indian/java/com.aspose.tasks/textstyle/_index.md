---
title: "TextStyle"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट दृश्य में आइटम के लिए टेक्स्ट की दृश्य शैली बदलें।"
type: docs
weight: 315
url: /hi/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

प्रोजेक्ट दृश्य में आइटम के लिए टेक्स्ट की दृश्य शैली बदलें।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TextStyle()](#TextStyle--) | डिफ़ॉल्ट सेटिंग्स के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है। |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट आकार और शैली के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है। |
| [TextStyle(int fontStyle)](#TextStyle-int-) | डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट शैली के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है। |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | निर्दिष्ट फ़ॉन्ट सेटिंग्स के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | टेक्स्ट शैली का पृष्ठभूमि रंग प्राप्त करता है। |
| [getBackgroundPattern()](#getBackgroundPattern--) | टेक्स्ट शैली का पृष्ठभूमि पैटर्न प्राप्त करता है। |
| [getColor()](#getColor--) | टेक्स्ट का रंग प्राप्त करता है। |
| [getFont()](#getFont--) | टेक्स्ट शैली का फ़ॉन्ट प्राप्त करता है। |
| [getItemType()](#getItemType--) | टेक्स्ट शैली का [TextItemType](../../com.aspose.tasks/textitemtype) प्राप्त करता है। |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | टेक्स्ट शैली का पृष्ठभूमि रंग सेट करता है। |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | टेक्स्ट शैली का पृष्ठभूमि पैटर्न सेट करता है। |
| [setColor(Color value)](#setColor-java.awt.Color-) | टेक्स्ट का रंग सेट करता है। |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | टेक्स्ट शैली का फ़ॉन्ट सेट करता है। |
| [setItemType(int value)](#setItemType-int-) | टेक्स्ट शैली का [TextItemType](../../com.aspose.tasks/textitemtype) सेट करता है। |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


डिफ़ॉल्ट सेटिंग्स के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है।

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट आकार और शैली के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontSize | float | TextStyle का फ़ॉन्ट आकार। |
| fontStyle | int | TextStyle का फ़ॉन्ट शैली। |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट शैली के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontStyle | int | डिफ़ॉल्ट फ़ॉन्ट पर लागू करने के लिए फ़ॉन्ट की शैली। |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


निर्दिष्ट फ़ॉन्ट सेटिंग्स के साथ [TextStyle](../../com.aspose.tasks/textstyle) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | टेक्स्ट स्टाइल का फ़ॉन्ट। |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


टेक्स्ट स्टाइल की पृष्ठभूमि रंग प्राप्त करता है। `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - टेक्स्ट स्टाइल की पृष्ठभूमि रंग।
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


टेक्स्ट स्टाइल का पृष्ठभूमि पैटर्न प्राप्त करता है। `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - टेक्स्ट स्टाइल का पृष्ठभूमि पैटर्न।
### getColor() {#getColor--}
```
public final Color getColor()
```


टेक्स्ट का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - टेक्स्ट का रंग।
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


टेक्स्ट शैली का फ़ॉन्ट प्राप्त करता है।

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


टेक्स्ट शैली का [TextItemType](../../com.aspose.tasks/textitemtype) प्राप्त करता है।

**Returns:**
int - टेक्स्ट स्टाइल का [TextItemType](../../com.aspose.tasks/textitemtype)।
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


टेक्स्ट स्टाइल की पृष्ठभूमि रंग सेट करता है। `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | टेक्स्ट स्टाइल की पृष्ठभूमि रंग। |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


टेक्स्ट स्टाइल का पृष्ठभूमि पैटर्न सेट करता है। `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | टेक्स्ट स्टाइल का पृष्ठभूमि पैटर्न। |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


टेक्स्ट का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | टेक्स्ट का रंग। |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


टेक्स्ट शैली का फ़ॉन्ट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | टेक्स्ट स्टाइल का फ़ॉन्ट। |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


टेक्स्ट शैली का [TextItemType](../../com.aspose.tasks/textitemtype) सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | टेक्स्ट स्टाइल का [TextItemType](../../com.aspose.tasks/textitemtype)। |

