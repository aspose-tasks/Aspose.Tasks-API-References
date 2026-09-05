---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पेजों को PDF में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 191
url: /hi/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

प्रोजेक्ट पेजों को PDF में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | एक नया उदाहरण प्रारंभ करता है [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) क्लास का, जिसका उपयोग दस्तावेज़ को [SaveFileFormat](../../com.aspose.tasks/savefileformat) फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर प्राप्त करता है। |
| [getEncryptionDetails()](#getEncryptionDetails--) | एन्क्रिप्शन विवरण प्राप्त करता है। |
| [getFontSettings()](#getFontSettings--) | प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है। |
| [getPageSavingCallback()](#getPageSavingCallback--) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक प्राप्त करता है। |
| [getPages()](#getPages--) | प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची प्राप्त करता है। |
| [getReduceFooterGap()](#getReduceFooterGap--) | अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है। |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getTextCompression()](#getTextCompression--) | छवियों को छोड़कर सभी कंटेंट स्ट्रीम्स के लिए उपयोग किए जाने वाले संपीड़न प्रकार को प्राप्त करता है। |
| [setCompliance(int value)](#setCompliance-int-) | जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर सेट करता है। |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | एन्क्रिप्शन विवरण सेट करता है। |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक सेट करता है। |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची सेट करता है। |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है। |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजना है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setTextCompression(int value)](#setTextCompression-int-) | छवियों को छोड़कर सभी कंटेंट स्ट्रीम्स के लिए उपयोग किए जाने वाले संपीड़न प्रकार को सेट करता है। |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


एक नया उदाहरण प्रारंभ करता है [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) क्लास का, जिसका उपयोग दस्तावेज़ को [SaveFileFormat](../../com.aspose.tasks/savefileformat) फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर प्राप्त करता है। डिफ़ॉल्ट है [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)।

**Returns:**
int - जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर।
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


एन्क्रिप्शन विवरण प्राप्त करता है। यदि सेट नहीं किया गया, तो कोई एन्क्रिप्शन नहीं किया जाएगा।

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है।

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


एक उपयोगकर्ता-परिभाषित कॉलबैक प्राप्त करता है जिसका उपयोग प्रत्येक रेंडर किए गए पृष्ठ के लिए आउटपुट स्ट्रीम प्राप्त करने के लिए किया जाता है। यह तब लागू होता है जब `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) विकल्प का उपयोग किया जाता है।

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची प्राप्त करता है।

--------------------

यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे।

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची।
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान।
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - यह मान दर्शाता है कि प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजा जाए या नहीं।
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


सभी कंटेंट स्ट्रीम्स (छवियों को छोड़कर) के लिए उपयोग किए जाने वाले संपीड़न प्रकार को प्राप्त करता है। डिफ़ॉल्ट है [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - सभी कंटेंट स्ट्रीम्स (छवियों को छोड़कर) के लिए उपयोग किया जाने वाला संपीड़न प्रकार।
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर सेट करता है। डिफ़ॉल्ट है [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | जेनरेट किए गए PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर। |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


एन्क्रिप्शन विवरण सेट करता है। यदि सेट नहीं किया गया, तो कोई एन्क्रिप्शन नहीं किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | एक एन्क्रिप्शन विवरण। |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


एक उपयोगकर्ता-परिभाषित कॉलबैक सेट करता है जिसका उपयोग प्रत्येक रेंडर किए गए पृष्ठ के लिए आउटपुट स्ट्रीम प्राप्त करने के लिए किया जाता है। यह तब लागू होता है जब `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) विकल्प उपयोग किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | एक उपयोगकर्ता-परिभाषित कॉलबैक जो प्रत्येक रेंडर किए गए पृष्ठ के लिए आउटपुट स्ट्रीम प्राप्त करने के लिए उपयोग किया जाता है। |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची सेट करता है।

--------------------

यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.List&lt;java.lang.Integer&gt; | प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची। |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं। |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजना है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि प्रोजेक्ट पृष्ठों को अलग फ़ाइलों में सहेजा जाए या नहीं। |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


सभी कंटेंट स्ट्रीम्स (छवियों को छोड़कर) के लिए उपयोग किए जाने वाले संपीड़न प्रकार को सेट करता है। डिफ़ॉल्ट है [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | सभी कंटेंट स्ट्रीम्स (छवियों को छोड़कर) के लिए उपयोग किया जाने वाला संपीड़न प्रकार। |

