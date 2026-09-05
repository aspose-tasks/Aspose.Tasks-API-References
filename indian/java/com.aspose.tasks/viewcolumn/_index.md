---
title: "ViewColumn"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट दृश्य में एक कॉलम को दर्शाता है।"
type: docs
weight: 344
url: /hi/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

प्रोजेक्ट दृश्य में एक कॉलम को दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getField()](#getField--) | कॉलम फ़ील्ड प्राप्त करता है। |
| [getName()](#getName--) | कॉलम का नाम प्राप्त करता है। |
| [getStringAlignment()](#getStringAlignment--) | पाठ का संरेखण प्राप्त करता है (यह [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) एनोमरेशन के मानों में से एक हो सकता है)। |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | कॉलबैक प्राप्त करता है जिसका उपयोग कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है। |
| [getWidth()](#getWidth--) | कॉलम की चौड़ाई प्राप्त करता है। |
| [setField(int value)](#setField-int-) | कॉलम फ़ील्ड सेट करता है। |
| [setStringAlignment(int value)](#setStringAlignment-int-) | पाठ की संरेखण सेट करता है (यह [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumeration के मानों में से एक हो सकता है)। |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | कॉलबैक सेट करता है जिसका उपयोग कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है। |
### getField() {#getField--}
```
public abstract int getField()
```


कॉलम फ़ील्ड प्राप्त करता है। `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - कॉलम फ़ील्ड।
### getName() {#getName--}
```
public final String getName()
```


कॉलम का नाम प्राप्त करता है।

**Returns:**
java.lang.String - कॉलम का नाम।
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


पाठ का संरेखण प्राप्त करता है (यह [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) एनोमरेशन के मानों में से एक हो सकता है)।

**Returns:**
int - पाठ की संरेखण (यह [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumeration के मानों में से एक हो सकता है)।
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


कॉलबैक प्राप्त करता है जिसका उपयोग कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है।

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


कॉलम की चौड़ाई प्राप्त करता है।

**Returns:**
int - कॉलम की चौड़ाई।
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


कॉलम फ़ील्ड सेट करता है। `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | कॉलम फ़ील्ड। |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


पाठ की संरेखण सेट करता है (यह [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumeration के मानों में से एक हो सकता है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | पाठ की संरेखण (यह [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumeration के मानों में से एक हो सकता है)। |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


कॉलबैक सेट करता है जिसका उपयोग कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | कॉलबैक जिसका उपयोग कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है। |

