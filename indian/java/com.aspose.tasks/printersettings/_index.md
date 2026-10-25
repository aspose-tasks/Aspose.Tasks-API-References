---
title: "PrinterSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "दस्तावेज़ कैसे प्रिंट किया जाता है, जिसमें प्रिंटर शामिल है, इसके बारे में जानकारी निर्दिष्ट करता है।"
type: docs
weight: 215
url: /hi/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

एक दस्तावेज़ कैसे प्रिंट किया जाता है, जिसमें प्रिंटर भी शामिल है, इस बारे में जानकारी निर्दिष्ट करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCollate()](#getCollate--) | प्रिंट किए गए दस्तावेज़ के कोलैटेड होने का संकेत देने वाला मान प्राप्त करता है। |
| [getCopies()](#getCopies--) | प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या प्राप्त करता है। |
| [getFromPage()](#getFromPage--) | प्रिंट करने के लिए पहले पृष्ठ का पृष्ठ संख्या प्राप्त करता है। |
| [getPrintFileName()](#getPrintFileName--) | फ़ाइल में प्रिंट करते समय फ़ाइल नाम प्राप्त करता है। |
| [getPrinterName()](#getPrinterName--) | उपयोग करने के लिए प्रिंटर का नाम प्राप्त करता है। |
| [getSupportsColor()](#getSupportsColor--) | यह प्रिंटर रंग प्रिंटिंग का समर्थन करता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getToPage()](#getToPage--) | प्रिंट करने के लिए अंतिम पृष्ठ की संख्या प्राप्त करता है। |
| [isDefaultPrinter()](#isDefaultPrinter--) | PrinterName प्रॉपर्टी डिफ़ॉल्ट प्रिंटर को निर्दिष्ट करती है या नहीं, यह दर्शाने वाला मान प्राप्त करता है, जब तक उपयोगकर्ता स्पष्ट रूप से PrinterName सेट नहीं करता। |
| [setCollate(boolean value)](#setCollate-boolean-) | प्रिंट किए गए दस्तावेज़ के कोलैटेड होने का संकेत देने वाला मान सेट करता है। |
| [setCopies(short value)](#setCopies-short-) | प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या सेट करता है। |
| [setFromPage(int value)](#setFromPage-int-) | प्रिंट करने के लिए पहले पृष्ठ की पृष्ठ संख्या सेट करता है। |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | फ़ाइल में प्रिंट करते समय फ़ाइल नाम सेट करता है। |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | उपयोग करने के लिए प्रिंटर का नाम सेट करता है। |
| [setToPage(int value)](#setToPage-int-) | प्रिंट करने के लिए अंतिम पृष्ठ की संख्या सेट करता है। |
| [toString()](#toString--) | PrinterSettings के बारे में जानकारी स्ट्रिंग रूप में प्रदान करता है। |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


प्रिंट किए गए दस्तावेज़ के कोलैटेड होने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - प्रिंट किए गए दस्तावेज़ के कोलैटेड होने का संकेत देने वाला मान।
### getCopies() {#getCopies--}
```
public short getCopies()
```


प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या प्राप्त करता है।

**Returns:**
short - प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या।
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


प्रिंट करने के लिए पहले पृष्ठ का पृष्ठ संख्या प्राप्त करता है।

**Returns:**
int - प्रिंट करने के लिए पहले पृष्ठ की पृष्ठ संख्या।
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


फ़ाइल में प्रिंट करते समय फ़ाइल नाम प्राप्त करता है।

**Returns:**
java.lang.String - फ़ाइल का नाम, जब फ़ाइल में प्रिंट किया जाता है।
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


उपयोग करने के लिए प्रिंटर का नाम प्राप्त करता है।

**Returns:**
java.lang.String - उपयोग करने वाले प्रिंटर का नाम।
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


यह प्रिंटर रंग प्रिंटिंग का समर्थन करता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि यह प्रिंटर रंगीन प्रिंटिंग का समर्थन करता है या नहीं।
### getToPage() {#getToPage--}
```
public int getToPage()
```


प्रिंट करने के लिए अंतिम पृष्ठ की संख्या प्राप्त करता है।

**Returns:**
int - प्रिंट करने के लिए अंतिम पृष्ठ की संख्या।
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


PrinterName प्रॉपर्टी डिफ़ॉल्ट प्रिंटर को निर्दिष्ट करती है या नहीं, यह दर्शाने वाला मान प्राप्त करता है, जब तक उपयोगकर्ता स्पष्ट रूप से PrinterName सेट नहीं करता।

**Returns:**
boolean - एक मान जो दर्शाता है कि PrinterName प्रॉपर्टी डिफ़ॉल्ट प्रिंटर को निर्दिष्ट करती है या नहीं।
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


प्रिंट किए गए दस्तावेज़ के कोलैटेड होने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि मुद्रित दस्तावेज़ क्रमबद्ध है या नहीं। |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | short | प्रिंट करने के लिए दस्तावेज़ की प्रतियों की संख्या। |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


प्रिंट करने के लिए पहले पृष्ठ की पृष्ठ संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | प्रिंट करने के लिए पहले पृष्ठ का पृष्ठ संख्या। |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


फ़ाइल में प्रिंट करते समय फ़ाइल नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | फ़ाइल का नाम, जब फ़ाइल में प्रिंट किया जाता है। |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


उपयोग करने के लिए प्रिंटर का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | उपयोग करने वाले प्रिंटर का नाम। |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


प्रिंट करने के लिए अंतिम पृष्ठ की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | प्रिंट करने के लिए अंतिम पृष्ठ की संख्या। |

### toString() {#toString--}
```
public String toString()
```


PrinterSettings के बारे में जानकारी स्ट्रिंग रूप में प्रदान करता है।

**Returns:**
java.lang.String - स्ट्रिंग रूप में PrinterSettings के बारे में जानकारी।
