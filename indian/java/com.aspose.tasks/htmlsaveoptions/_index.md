---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पृष्ठों को HTML में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 132
url: /hi/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

प्रोजेक्ट पृष्ठों को HTML में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | एक नया उदाहरण प्रारंभ करता है [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | CSS को संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है। |
| [getCssStylePrefix()](#getCssStylePrefix--) | CSS शैली उपसर्ग प्राप्त करता है। |
| [getExportCss()](#getExportCss--) | CSS निर्यात करने का तरीका प्राप्त करता है। |
| [getExportFonts()](#getExportFonts--) | फ़ॉन्ट निर्यात करने का तरीका प्राप्त करता है। |
| [getExportImages()](#getExportImages--) | छवियों को निर्यात करने का तरीका प्राप्त करता है। |
| [getFontFaceTypes()](#getFontFaceTypes--) | फ़ॉन्ट फेस प्रकार प्राप्त करता है। |
| [getFontSavingCallback()](#getFontSavingCallback--) | फ़ॉन्ट संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है। |
| [getFontSettings()](#getFontSettings--) | प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है। |
| [getImageSavingCallback()](#getImageSavingCallback--) | फ़ॉन्ट संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है। |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | HTML पेज हेडर में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान प्राप्त करता है। |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | HTML शीर्षक में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान प्राप्त करता है। |
| [getPageSavingCallback()](#getPageSavingCallback--) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक प्राप्त करता है। |
| [getPages()](#getPages--) | प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पेज नंबरों की सूची प्राप्त करता है। |
| [getReduceFooterGap()](#getReduceFooterGap--) | अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है। |
| [getUseGradientBrush()](#getUseGradientBrush--) | प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश उपयोग करने का संकेत देने वाला मान प्राप्त करता है। |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | CSS को संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को सेट करता है। |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | CSS शैली उपसर्ग सेट करता है। |
| [setExportCss(int value)](#setExportCss-int-) | CSS निर्यात करने का तरीका सेट करता है। |
| [setExportFonts(int value)](#setExportFonts-int-) | फ़ॉन्ट निर्यात करने का तरीका सेट करता है। |
| [setExportImages(int value)](#setExportImages-int-) | छवियों को निर्यात करने का तरीका सेट करता है। |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | फ़ॉन्ट फ़ेस प्रकार सेट करता है। |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए कॉल किए जाने वाले कॉलबैक को सेट करता है। |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए कॉल किए जाने वाले कॉलबैक को सेट करता है। |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | HTML पेज हेडर में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान सेट करता है। |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | HTML शीर्षक में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान सेट करता है। |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने हेतु उपयोग किया जाने वाला उपयोगकर्ता-परिभाषित कॉलबैक सेट करता है। |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पेज नंबरों की सूची सेट करता है। |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है। |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश उपयोग करने का संकेत देने वाला मान सेट करता है। |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


एक नया उदाहरण प्रारंभ करता है [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) क्लास का।

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


CSS को संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है।

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


CSS शैली उपसर्ग प्राप्त करता है।

**Returns:**
java.lang.String - CSS शैली उपसर्ग।
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


CSS निर्यात करने का तरीका प्राप्त करता है।

**Returns:**
int - CSS निर्यात करने का तरीका।
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


फ़ॉन्ट निर्यात करने का तरीका प्राप्त करता है।

**Returns:**
int - फ़ॉन्ट निर्यात करने का तरीका।
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


छवियों को निर्यात करने का तरीका प्राप्त करता है।

**Returns:**
int - छवियों को निर्यात करने का तरीका।
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


फ़ॉन्ट फेस प्रकार प्राप्त करता है।

मान: फ़ॉन्ट फ़ेस प्रकार।

**Returns:**
int - फ़ॉन्ट फ़ेस प्रकार।
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


फ़ॉन्ट संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है।

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है।

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


फ़ॉन्ट संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को प्राप्त करता है।

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


HTML पेज हेडर में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - HTML पेज हेडर में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान।
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


HTML शीर्षक में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - HTML शीर्षक में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान।
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


प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पेज नंबरों की सूची प्राप्त करता है।

--------------------

यदि यह सूची खाली है तो सभी प्रोजेक्ट पेज सहेजे जाएंगे।

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पेज नंबरों की सूची।
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


अंतिम टास्क और फुटर के बीच अंतराल को कम करने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान।
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश उपयोग करने का संकेत देने वाला मान प्राप्त करता है।

--------------------

HTML में रेंडर करते समय ग्रेडिएंट ब्रश का वर्तमान उपयोग समर्थित नहीं है।

**Returns:**
boolean - प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश उपयोग करने का संकेत देने वाला मान।
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


CSS को संग्रहीत करने के लिए संसाधन बनाने वाले कॉलबैक को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | CSS संग्रहीत करने के संसाधन को बनाने के लिए कॉल किए जाने वाले कॉलबैक। |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


CSS शैली उपसर्ग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | CSS शैली उपसर्ग। |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


CSS निर्यात करने का तरीका सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | CSS निर्यात किए जाने का तरीका। |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


फ़ॉन्ट निर्यात करने का तरीका सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़ॉन्ट निर्यात किए जाने का तरीका। |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


छवियों को निर्यात करने का तरीका सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | छवियों का निर्यात किया जाने का तरीका। |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


फ़ॉन्ट फ़ेस प्रकार सेट करता है।

मान: फ़ॉन्ट फ़ेस प्रकार।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़ॉन्ट फ़ेस प्रकार। |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए कॉल किए जाने वाले कॉलबैक को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए बुलाए जाने वाला कॉलबैक। |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए कॉल किए जाने वाले कॉलबैक को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | फ़ॉन्ट संग्रहीत करने के संसाधन को बनाने के लिए बुलाए जाने वाला कॉलबैक। |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


HTML पेज हेडर में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि HTML पेज हेडर में प्रोजेक्ट नाम शामिल किया जाए या नहीं। |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


HTML शीर्षक में प्रोजेक्ट नाम शामिल करने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि HTML शीर्षक में प्रोजेक्ट नाम शामिल किया जाए या नहीं। |

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


प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पेज नंबरों की सूची सेट करता है।

--------------------

यदि यह सूची खाली है तो सभी प्रोजेक्ट पेज सहेजे जाएंगे।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.List&lt;java.lang.Integer&gt; | प्रोजेक्ट लेआउट रेंडर करते समय सहेजने के लिए पृष्ठ संख्याओं की सूची। |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


अंतिम कार्य और फ़ूटर के बीच अंतराल को घटाने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं। |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश उपयोग करने का संकेत देने वाला मान सेट करता है।

--------------------

HTML में रेंडर करते समय ग्रेडिएंट ब्रश का वर्तमान उपयोग समर्थित नहीं है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो इंगित करता है कि प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं। |

