---
title: "TableTextStyle"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "व्यू तालिका में एक टेक्स्ट शैली का प्रतिनिधित्व करता है।"
type: docs
weight: 288
url: /hi/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

व्यू तालिका में एक टेक्स्ट शैली का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | निर्दिष्ट फ़ॉन्ट के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | निर्दिष्ट फ़ॉन्ट आकार और फ़ॉन्ट शैली के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | डिफ़ॉल्ट फ़ॉन्ट सेटिंग्स और निर्दिष्ट फ़ॉन्ट शैली के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getField()](#getField--) | उस फ़ील्ड को प्राप्त करता है जिस पर शैली लागू की जानी है। |
| [getItemType()](#getItemType--) | टेक्स्ट आइटम प्रकार लौटाता है। |
| [getRowUid()](#getRowUid--) | एक पंक्ति का यूनिक आईडी प्राप्त करता है। |
| [setField(int value)](#setField-int-) | उस फ़ील्ड को सेट करता है जिस पर शैली लागू की जानी है। |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


[TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | int | एक निर्दिष्ट पंक्ति यूनिक आईडी। |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


निर्दिष्ट फ़ॉन्ट के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | int | एक निर्दिष्ट पंक्ति यूनिक आईडी। |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | एक फ़ॉन्ट जिस पर टेक्स्ट शैली आधारित है। |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


निर्दिष्ट फ़ॉन्ट आकार और फ़ॉन्ट शैली के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | int | एक निर्दिष्ट पंक्ति यूनिक आईडी। |
| fontSize | float | फ़ॉन्ट का आकार जिस पर टेक्स्ट शैली आधारित है। |
| fontStyle | int | फ़ॉन्ट शैली। |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


डिफ़ॉल्ट फ़ॉन्ट सेटिंग्स और निर्दिष्ट फ़ॉन्ट शैली के साथ [TableTextStyle](../../com.aspose.tasks/tabletextstyle) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | int | एक निर्दिष्ट पंक्ति यूनिक आईडी। |
| fontStyle | int | फ़ॉन्ट शैली। |

### getField() {#getField--}
```
public final int getField()
```


उस फ़ील्ड को प्राप्त करता है जिस पर शैली लागू की जानी है। `Field`([getField()](../../com.aspose/tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose/tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - वह फ़ील्ड जिस पर शैली लागू की जानी है।
### getItemType() {#getItemType--}
```
public int getItemType()
```


टेक्स्ट आइटम प्रकार लौटाता है।

**Returns:**
int - TextItemType एन्यूमरेटेड टाइप मान।
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


एक पंक्ति का यूनिक आईडी प्राप्त करता है।

--------------------

यदि शैली को दृश्य की सभी पंक्तियों पर लागू करना हो तो -1 लौटाएँ।

**Returns:**
int - पंक्ति का अद्वितीय आईडी।
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


उस फ़ील्ड को सेट करता है जिस पर शैली लागू की जानी है। `Field`([getField()](../../com.aspose/tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose/tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक फ़ील्ड जिस पर शैली लागू की जानी है। |

