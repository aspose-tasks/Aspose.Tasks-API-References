---
title: "Filter"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "परियोजना में एक फ़िल्टर को दर्शाता है।"
type: docs
weight: 91
url: /hi/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

परियोजना में एक फ़िल्टर को दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Filter()](#Filter--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | इस उदाहरण की तुलना निर्दिष्ट [Filter](../../com.aspose.tasks/filter) क्लास के उदाहरण से करता है और उनके सापेक्ष क्रम का संकेत लौटाता है। |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं। |
| [getCriteria()](#getCriteria--) | MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करनी वाली मानदंड प्राप्त करता है। |
| [getFilterType()](#getFilterType--) | फ़िल्टर का प्रकार प्राप्त करता है। |
| [getIndex()](#getIndex--) | Filters समाहित वस्तु में एक [Filter](../../com.aspose.tasks/filter) ऑब्जेक्ट का सूचकांक प्राप्त करता है। |
| [getName()](#getName--) | एक Filter ऑब्जेक्ट का नाम प्राप्त करता है। |
| [getShowInMenu()](#getShowInMenu--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट रिबन के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं। |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | एक मान प्राप्त करता है जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं। |
| [getUid()](#getUid--) | फ़िल्टर का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [hashCode()](#hashCode--) | फ़िल्टर के लिए हैश कोड मान लौटाता है। |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करना आवश्यक मानदंड सेट करता है। |
| [setFilterType(int value)](#setFilterType-int-) | फ़िल्टर का प्रकार। |
| [setName(String value)](#setName-java.lang.String-) | एक Filter ऑब्जेक्ट का नाम सेट करता है। |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट रिबन के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं। |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | एक मान सेट करता है जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं। |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


इस उदाहरण की तुलना निर्दिष्ट [Filter](../../com.aspose.tasks/filter) क्लास के उदाहरण से करता है और उनके सापेक्ष क्रम का संकेत लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | इस ऑब्जेक्ट से तुलना करने के लिए निर्दिष्ट [Filter](../../com.aspose.tasks/filter) क्लास का इंस्टेंस। |

**Returns:**
int - उनके सापेक्ष क्रम का संकेत।
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट AssignmentBaseline ऑब्जेक्ट। |

**Returns:**
boolean - true लौटाता है यदि यह इंस्टेंस निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है; अन्यथा, false।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट AssignmentBaseline ऑब्जेक्ट। |

**Returns:**
boolean - true लौटाता है यदि यह इंस्टेंस निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है; अन्यथा, false।
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करनी वाली मानदंड प्राप्त करता है।

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


फ़िल्टर का प्रकार प्राप्त करता है।

**Returns:**
int - फ़िल्टर का प्रकार।
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Filters समाहित वस्तु में एक [Filter](../../com.aspose.tasks/filter) ऑब्जेक्ट का सूचकांक प्राप्त करता है।

**Returns:**
int - Filters समाहित वस्तु में एक [Filter](../../com.aspose.tasks/filter) ऑब्जेक्ट का सूचकांक।
### getName() {#getName--}
```
public final String getName()
```


एक Filter ऑब्जेक्ट का नाम प्राप्त करता है।

**Returns:**
java.lang.String - एक Filter ऑब्जेक्ट का नाम।
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट रिबन के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं।

**Returns:**
boolean - वह मान जो दर्शाता है कि प्रोजेक्ट Ribbon के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं।
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


एक मान प्राप्त करता है जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं।

**Returns:**
boolean - वह मान जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं।
### getUid() {#getUid--}
```
public final int getUid()
```


फ़िल्टर का अद्वितीय पहचानकर्ता प्राप्त करता है।

**Returns:**
int - फ़िल्टर का अद्वितीय पहचानकर्ता।
### hashCode() {#hashCode--}
```
public int hashCode()
```


फ़िल्टर के लिए हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | पहला फ़िल्टर। |
| b | [Filter](../../com.aspose.tasks/filter) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करना आवश्यक मानदंड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | वे मानदंड जिनको कार्य या संसाधनों को MSP दृश्य में प्रदर्शित होने के लिए पूरा करना आवश्यक है। |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


फ़िल्टर का प्रकार।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | फ़िल्टर का प्रकार। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


एक Filter ऑब्जेक्ट का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | फ़िल्टर ऑब्जेक्ट का नाम। |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट रिबन के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि प्रोजेक्ट Ribbon के View टैब पर Filter ड्रॉप-डाउन सूची में फ़िल्टर नाम दिखाता है या नहीं। |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि फ़िल्टर के लिए संबंधित सारांश पंक्तियाँ प्रदर्शित की गई हैं या नहीं। |

