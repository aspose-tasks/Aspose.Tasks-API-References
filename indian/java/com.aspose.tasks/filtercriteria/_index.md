---
title: "FilterCriteria"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करने वाले मानदंड को परिभाषित करता है।"
type: docs
weight: 94
url: /hi/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करने वाले मानदंड को परिभाषित करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | बच्चे [FilterCriteria](../../com.aspose.tasks/filtercriteria) पंक्तियों की सूची प्राप्त करता है। |
| [getField()](#getField--) | एक `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) को बदलने के लिए प्राप्त करता है। |
| [getOperation()](#getOperation--) | फ़िल्टर में अन्य मानदंडों से संबंधित, FieldName, Test और Value के साथ स्थापित मानदंड को प्राप्त करता है। |
| [getTest()](#getTest--) | फ़िल्टर के चयन मानदंड के रूप में कार्य करने वाले, FieldName और Value के बीच किए गए तुलना प्रकार को प्राप्त करता है। |
| [getValues()](#getValues--) | FieldName के साथ निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए ऑब्जेक्ट मानों को प्राप्त करता है। |
| [isValueAField()](#isValueAField--) | यह प्राप्त करता है कि FilterCriteria का दाएँ हाथ का मान फ़ील्ड संदर्भ है, स्थिर मान नहीं। |
| [isValueAField(int index)](#isValueAField-int-) | यह प्राप्त करता है कि FilterCriteria के सूचकांक पर मान फ़ील्ड संदर्भ है, स्थिर मान नहीं। |
| [setField(int value)](#setField-int-) | एक `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) को बदलने के लिए सेट करता है। |
| [setOperation(int value)](#setOperation-int-) | फ़िल्टर में अन्य मानदंडों से संबंधित, FieldName, Test और Value के साथ स्थापित मानदंड को सेट करता है। |
| [setTest(int value)](#setTest-int-) | फ़िल्टर के चयन मानदंड के रूप में कार्य करने वाले, FieldName और Value के बीच किए गए तुलना प्रकार को सेट करता है। |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए सूचकांक पर ऑब्जेक्ट मान को सेट करता है। |
| [setValue(Object value)](#setValue-java.lang.Object-) | FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए ऑब्जेक्ट मान को सेट करता है। |
| [setValueByField(int value)](#setValueByField-int-) | फ़ील्ड को सेट करता है जिसका मान FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना किया जाएगा। |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | सूचकांक पर फ़ील्ड को सेट करता है जिसका मान FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना किया जाएगा। |
| [toString()](#toString--) | [FilterCriteria](../../com.aspose.tasks/filtercriteria) वर्ग की इंस्टेंस की स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


बच्चे [FilterCriteria](../../com.aspose.tasks/filtercriteria) पंक्तियों की सूची प्राप्त करता है। यदि फ़िल्टर में एक से अधिक मानदंड पंक्तियाँ हैं तो And ऑपरेटर का प्रभाव यह है कि दोनों पंक्तियों के मानदंड पूरे होने चाहिए ताकि कार्य या संसाधन इस फ़िल्टर के परिणामस्वरूप प्रदर्शित हो। Or ऑपरेटर का प्रभाव यह है कि किसी एक पंक्ति के मानदंड पूरे होने चाहिए।

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - बच्चे [FilterCriteria](../../com.aspose.tasks/filtercriteria) पंक्तियों की सूची।
### getField() {#getField--}
```
public final int getField()
```


एक `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) को बदलने के लिए प्राप्त करता है।

**Returns:**
int - एक `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) को बदलने के लिए।
### getOperation() {#getOperation--}
```
public final int getOperation()
```


फ़िल्टर में अन्य मानदंडों से संबंधित, FieldName, Test और Value के साथ स्थापित मानदंड को प्राप्त करता है।

**Returns:**
int - फ़िल्टर में अन्य मानदंडों से संबंधित, FieldName, Test और Value के साथ स्थापित मानदंड।
### getTest() {#getTest--}
```
public final int getTest()
```


फ़िल्टर के चयन मानदंड के रूप में कार्य करने वाले, FieldName और Value के बीच किए गए तुलना प्रकार को प्राप्त करता है। [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - फ़िल्टर के चयन मानदंड के रूप में कार्य करने वाले, FieldName और Value के बीच किए गए तुलना प्रकार।
### getValues() {#getValues--}
```
public final Object[] getValues()
```


FieldName के साथ निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए ऑब्जेक्ट मानों को प्राप्त करता है।

**Returns:**
java.lang.Object[] - FieldName के साथ निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए ऑब्जेक्ट मान।
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


यह प्राप्त करता है कि FilterCriteria का दाएँ हाथ का मान फ़ील्ड संदर्भ है, स्थिर मान नहीं।

**Returns:**
boolean - यह कि FilterCriteria का दाएँ हाथ का मान फ़ील्ड संदर्भ है, स्थिर मान नहीं।
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


यह प्राप्त करता है कि FilterCriteria के सूचकांक पर मान फ़ील्ड संदर्भ है, स्थिर मान नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | मान का सूचकांक |

**Returns:**
बूलियन - यह कि FilterCriteria के इंडेक्स पर दाएँ हाथ का मान एक फ़ील्ड रेफ़रेंस है, स्थायी मान नहीं।
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


एक `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) को बदलने के लिए सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | बदलने के लिए एक `Field`([getField()](../../com.aspose/tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))। |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


फ़िल्टर में अन्य मानदंडों से संबंधित, FieldName, Test और Value के साथ स्थापित मानदंड को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़िल्टर में FieldName, Test, और Value के साथ स्थापित मानदंड अन्य मानदंडों से संबंधित है। |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


फ़िल्टर के लिए चयन मानदंड के रूप में कार्य करने वाले FieldName और Value के बीच किए गए तुलना प्रकार को सेट करता है। [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़िल्टर के लिए चयन मानदंड के रूप में कार्य करने वाले FieldName और Value के बीच किए गए तुलना प्रकार। |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए सूचकांक पर ऑब्जेक्ट मान को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | मान का इंडेक्स। |
| मान | java.lang.Object | ऑब्जेक्ट मान जो फ़िल्टर मानदंड के इंडेक्स पर दाएँ हाथ का मान प्रदान करेगा। |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना करने के लिए ऑब्जेक्ट मान को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.Object | ऑब्जेक्ट मान जो फ़िल्टर मानदंड का दाएँ हाथ का मान प्रदान करेगा। |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


फ़ील्ड को सेट करता है जिसका मान FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़ील्ड जो फ़िल्टर मानदंड का दाएँ हाथ का मान प्रदान करेगा। |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


सूचकांक पर फ़ील्ड को सेट करता है जिसका मान FieldName द्वारा निर्दिष्ट फ़ील्ड के मान से तुलना किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | मान का सूचकांक |
| मान | int | फ़ील्ड जो फ़िल्टर मानदंड के इंडेक्स पर दाएँ हाथ का मान प्रदान करेगा। |

### toString() {#toString--}
```
public String toString()
```


[FilterCriteria](../../com.aspose.tasks/filtercriteria) वर्ग की इंस्टेंस की स्ट्रिंग प्रतिनिधित्व लौटाता है।

**Returns:**
java.lang.String - इस वस्तु का स्ट्रिंग प्रतिनिधित्व।
