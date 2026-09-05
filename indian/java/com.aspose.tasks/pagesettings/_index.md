---
title: "PageSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट व्यू के पेज के लिए प्रिंटिंग सेटिंग्स का प्रतिनिधित्व करता है।"
type: docs
weight: 181
url: /hi/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

प्रोजेक्ट व्यू के पेज के लिए प्रिंटिंग सेटिंग्स का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PageSettings()](#PageSettings--) | नए [PageSettings](../../com.aspose.tasks/pagesettings) क्लास का एक नया उदाहरण इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | निर्धारित प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) पर प्रिंटिंग को समायोजित करने के लिए एक मान प्राप्त करता है। |
| [getFirstPageNumber()](#getFirstPageNumber--) | प्रिंटिंग के लिए पहला पृष्ठ क्रमांक प्राप्त करता है। |
| [getPagesInHeight()](#getPagesInHeight--) | प्रिंट करने के लिए ऊँचाई में पृष्ठों की संख्या प्राप्त करता है। |
| [getPagesInWidth()](#getPagesInWidth--) | प्रिंट करने के लिए चौड़ाई में पृष्ठों की संख्या प्राप्त करता है। |
| [getPaperSize()](#getPaperSize--) | कागज़ का आकार प्राप्त करता है। |
| [getPaperSizeId()](#getPaperSizeId--) | PrinterPaperSize मानों में से एक या कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक प्राप्त करता है। |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत प्राप्त करता है। |
| [isPortrait()](#isPortrait--) | पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है। |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | निर्धारित प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) पर प्रिंटिंग को समायोजित करने के लिए एक मान सेट करता है। |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | प्रिंटिंग के लिए पहला पृष्ठ क्रमांक सेट करता है। |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | ऊँचाई में प्रिंट होने वाले पृष्ठों की संख्या सेट करता है। |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | चौड़ाई में प्रिंट होने वाले पृष्ठों की संख्या सेट करता है। |
| [setPaperSize(int value)](#setPaperSize-int-) | कागज़ का आकार सेट करता है। |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | PrinterPaperSize मानों में से एक या कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक सेट करता है। |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत सेट करता है। |
| [setPortrait(boolean value)](#setPortrait-boolean-) | पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है। |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


नए [PageSettings](../../com.aspose/tasks/pagesettings) वर्ग का एक नया उदाहरण आरंभ करता है। प्रोजेक्ट दृश्य के पृष्ठ के लिए प्रिंटिंग सेटिंग्स का प्रतिनिधित्व करता है।

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


निर्धारित प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) पर प्रिंटिंग को समायोजित करने के लिए एक मान प्राप्त करता है।

--------------------

जब प्रोजेक्ट को HTML स्वरूप में रेंडर किया जाता है तो यह प्रभावी नहीं होता।

**Returns:**
boolean - निर्धारित प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) पर प्रिंटिंग को समायोजित करने के लिए एक मान।
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


प्रिंटिंग के लिए पहला पृष्ठ क्रमांक प्राप्त करता है।

**Returns:**
short - प्रिंटिंग के लिए पहला पृष्ठ क्रमांक।
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


प्रिंट करने के लिए ऊँचाई में पृष्ठों की संख्या प्राप्त करता है।

**Returns:**
int - ऊँचाई में प्रिंट होने वाले पृष्ठों की संख्या।
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


प्रिंट करने के लिए चौड़ाई में पृष्ठों की संख्या प्राप्त करता है।

**Returns:**
int - चौड़ाई में प्रिंट होने वाले पृष्ठों की संख्या।
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


कागज़ का आकार प्राप्त करता है। यह [PrinterPaperSize](../../com.aspose/tasks/printerpapersize) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - कागज़ का आकार।
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


PrinterPaperSize मानों में से एक या कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक प्राप्त करता है। इस मान का उपयोग OS सेटिंग्स से PaperSize प्राप्त करने के लिए किया जा सकता है।

**Returns:**
int - PrinterPaperSize मानों में से एक या एक कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक।
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत प्राप्त करता है।

**Returns:**
int - प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत।
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।

--------------------

जब SaveOptions.getPageSize() == PageSize.DefinedInView हो, तब रेंडरिंग के दौरान लागू होता है।

**Returns:**
boolean - यह दर्शाने वाला मान कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है।
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


निर्धारित प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) पर प्रिंटिंग को समायोजित करने के लिए एक मान सेट करता है।

--------------------

जब प्रोजेक्ट को HTML स्वरूप में रेंडर किया जाता है तो यह प्रभावी नहीं होता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | boolean | निर्दिष्ट प्रतिशत (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) के अनुसार सामान्य आकार को समायोजित करने का संकेत देने वाला मान। |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


प्रिंटिंग के लिए पहला पृष्ठ क्रमांक सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | short | प्रिंटिंग के लिए पहला पेज नंबर। |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


ऊँचाई में प्रिंट होने वाले पृष्ठों की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | ऊँचाई में प्रिंट किए जाने वाले पेजों की संख्या। |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


चौड़ाई में प्रिंट होने वाले पृष्ठों की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | चौड़ाई में प्रिंट किए जाने वाले पेजों की संख्या। |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


एक पेपर आकार सेट करता है। यह [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) एनेमरेशन के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक पेपर आकार। |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


PrinterPaperSize मानों में से एक या एक कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक सेट करता है। इस मान का उपयोग OS सेटिंग्स से PaperSize प्राप्त करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | PrinterPaperSize मानों में से एक या एक कस्टम पेज आकार आईडी को दर्शाने वाला पूर्णांक। |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत। |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।

--------------------

जब SaveOptions.getPageSize() == PageSize.DefinedInView हो, तब रेंडरिंग के दौरान लागू होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | पेज अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है। |

