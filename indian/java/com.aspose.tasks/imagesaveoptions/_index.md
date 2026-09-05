---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पृष्ठों को छवियों में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 134
url: /hi/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

प्रोजेक्ट पृष्ठों को छवियों में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | एक नया उदाहरण प्रारंभ करता है [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) वर्ग का, जिसका उपयोग रेंडर की गई छवियों को TIFF, PNG, BMP या JPEG स्वरूपों में सहेजने के लिए किया जा सकता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है। |
| [getHorizontalResolution()](#getHorizontalResolution--) | क्षैतिज रिज़ॉल्यूशन dpi में प्राप्त करता है। |
| [getJpegQuality()](#getJpegQuality--) | JPEG गुणवत्ता प्राप्त करता है। |
| [getPageSavingCallback()](#getPageSavingCallback--) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक प्राप्त करता है। |
| [getPages()](#getPages--) | प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची प्राप्त करता है। |
| [getPixelFormat()](#getPixelFormat--) | छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप प्राप्त करता है। |
| [getReduceFooterGap()](#getReduceFooterGap--) | अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है। |
| [getTiffCompression()](#getTiffCompression--) | TIFF स्वरूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न प्रकार प्राप्त करता है। |
| [getVerticalResolution()](#getVerticalResolution--) | ऊर्ध्वाधर रिज़ॉल्यूशन dpi में प्राप्त करता है। |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | क्षैतिज रिज़ॉल्यूशन dpi में सेट करता है। |
| [setJpegQuality(int value)](#setJpegQuality-int-) | JPEG गुणवत्ता सेट करता है। |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक सेट करता है। |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची सेट करता है। |
| [setPixelFormat(int value)](#setPixelFormat-int-) | छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप सेट करता है। |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है। |
| [setTiffCompression(int value)](#setTiffCompression-int-) | TIFF स्वरूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न प्रकार सेट करता है। |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | ऊर्ध्वाधर रिज़ॉल्यूशन dpi में सेट करता है। |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


एक नया उदाहरण प्रारंभ करता है [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) वर्ग का, जिसका उपयोग रेंडर की गई छवियों को TIFF, PNG, BMP या JPEG स्वरूपों में सहेजने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| saveFormat | int | TIFF, PNG, BMP या JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat) हो सकता है। |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


आंतरिक उपयोग के लिए आरक्षित।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


आंतरिक उपयोग के लिए आरक्षित।

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है।

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


क्षैतिज रिज़ॉल्यूशन dpi में प्राप्त करता है।

**Returns:**
float - क्षैतिज रिज़ॉल्यूशन dpi में।
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


JPEG गुणवत्ता प्राप्त करता है। अनुमत मान सीमा 0..100 है।

**Returns:**
int - JPEG गुणवत्ता।
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक प्राप्त करता है।

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची प्राप्त करता है।

--------------------

यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे।

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची।
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप प्राप्त करता है।

**Returns:**
int - छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप।
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान।
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


TIFF स्वरूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न प्रकार प्राप्त करता है।

--------------------

केवल TIFF में सहेजते समय प्रभावी होता है। डिफ़ॉल्ट मान `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\\#setTiffCompression-int-)) है।

**Returns:**
int - TIFF स्वरूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न प्रकार।
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


ऊर्ध्वाधर रिज़ॉल्यूशन dpi में प्राप्त करता है।

**Returns:**
float - ऊर्ध्वाधर रिज़ॉल्यूशन dpi में।
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


क्षैतिज रिज़ॉल्यूशन dpi में सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | float | डॉट्स प्रति इंच (dpi) में क्षैतिज रिज़ॉल्यूशन। |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


JPEG गुणवत्ता सेट करता है। अनुमत मान सीमा 0..100 है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक JPEG गुणवत्ता। |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | एक उपयोगकर्ता-परिभाषित कॉलबैक जो प्रत्येक रेंडर किए गए पृष्ठ के लिए आउटपुट स्ट्रीम प्राप्त करने के लिए उपयोग किया जाता है। |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची सेट करता है।

--------------------

यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.List&lt;java.lang.Integer&gt; | प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची। |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | छवि में प्रत्येक पिक्सेल के लिए रंग डेटा का प्रारूप। |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं। |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


TIFF स्वरूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न प्रकार सेट करता है।

--------------------

केवल TIFF में सहेजते समय प्रभावी होता है। डिफ़ॉल्ट मान `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\\#setTiffCompression-int-)) है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | TIFF प्रारूप में उत्पन्न छवियों को सहेजते समय लागू करने के लिए संपीड़न का प्रकार। |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


ऊर्ध्वाधर रिज़ॉल्यूशन dpi में सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | float | डॉट्स प्रति इंच (dpi) में ऊर्ध्वाधर रिज़ॉल्यूशन। |

