---
title: "Group"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "समूह परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 122
url: /hi/java/com.aspose.tasks/group/
---

**Inheritance:**
java.lang.Object
```
public class Group
```

एक समूह परिभाषा का प्रतिनिधित्व करता है। एक Group ऑब्जेक्ट ResourceGroups संग्रह या TaskGroups संग्रह का सदस्य होता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Group()](#Group--) | एक नया [Group](../../com.aspose.tasks/group) क्लास का इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getGroupAssignments()](#getGroupAssignments--) | एक मान प्राप्त करता है जो दर्शाता है कि असाइनमेंट्स को टास्क के बजाय समूहित किया जाना चाहिए या नहीं। |
| [getGroupCriteria()](#getGroupCriteria--) | एक GroupCriteria संग्रह प्राप्त करता है जो समूह परिभाषा में फ़ील्ड्स को दर्शाता है। |
| [getMaintainHierarchy()](#getMaintainHierarchy--) | एक मान प्राप्त करता है जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के समरी टास्क दिखाए जाएँ या नहीं। |
| [getName()](#getName--) | एक Group ऑब्जेक्ट का नाम प्राप्त करता है। |
| [getShowInMenu()](#getShowInMenu--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं। |
| [getShowSummary()](#getShowSummary--) | एक मान प्राप्त करता है जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं। |
| [getUid()](#getUid--) | एक समूह की विशिष्ट पहचानकर्ता प्राप्त करता है। |
| [setGroupAssignments(boolean value)](#setGroupAssignments-boolean-) | एक मान सेट करता है जो दर्शाता है कि असाइनमेंट को कार्यों के बजाय समूहित किया जाना चाहिए या नहीं। |
| [setGroupCriteria(GroupCriterionCollection value)](#setGroupCriteria-com.aspose.tasks.GroupCriterionCollection-) | एक GroupCriteria संग्रह सेट करता है जो समूह परिभाषा में फ़ील्ड्स को दर्शाता है। |
| [setMaintainHierarchy(boolean value)](#setMaintainHierarchy-boolean-) | एक मान सेट करता है जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के सारांश कार्य दिखाए जाएँ या नहीं। |
| [setName(String value)](#setName-java.lang.String-) | एक Group ऑब्जेक्ट का नाम सेट करता है। |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं। |
| [setShowSummary(boolean value)](#setShowSummary-boolean-) | एक मान सेट करता है जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं। |
### Group() {#Group--}
```
public Group()
```


एक नया [Group](../../com.aspose.tasks/group) क्लास का इंस्टेंस इनिशियलाइज़ करता है।

### getGroupAssignments() {#getGroupAssignments--}
```
public final boolean getGroupAssignments()
```


एक मान प्राप्त करता है जो दर्शाता है कि असाइनमेंट्स को टास्क के बजाय समूहित किया जाना चाहिए या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि असाइनमेंट को कार्यों के बजाय समूहित किया जाना चाहिए या नहीं।
### getGroupCriteria() {#getGroupCriteria--}
```
public final GroupCriterionCollection getGroupCriteria()
```


एक GroupCriteria संग्रह प्राप्त करता है जो समूह परिभाषा में फ़ील्ड्स को दर्शाता है।

**Returns:**
[GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) - a GroupCriteria collection representing the fields in a group definition.
### getMaintainHierarchy() {#getMaintainHierarchy--}
```
public final boolean getMaintainHierarchy()
```


एक मान प्राप्त करता है जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के समरी टास्क दिखाए जाएँ या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के सारांश कार्य दिखाए जाएँ या नहीं।
### getName() {#getName--}
```
public final String getName()
```


एक Group ऑब्जेक्ट का नाम प्राप्त करता है।

**Returns:**
java.lang.String - एक Group ऑब्जेक्ट का नाम।
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं।
### getShowSummary() {#getShowSummary--}
```
public final boolean getShowSummary()
```


एक मान प्राप्त करता है जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं।
### getUid() {#getUid--}
```
public final int getUid()
```


एक समूह की विशिष्ट पहचानकर्ता प्राप्त करता है।

**Returns:**
int - एक समूह की विशिष्ट पहचानकर्ता।
### setGroupAssignments(boolean value) {#setGroupAssignments-boolean-}
```
public final void setGroupAssignments(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि असाइनमेंट को कार्यों के बजाय समूहित किया जाना चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि असाइनमेंट को कार्यों के बजाय समूहित किया जाना चाहिए या नहीं। |

### setGroupCriteria(GroupCriterionCollection value) {#setGroupCriteria-com.aspose.tasks.GroupCriterionCollection-}
```
public final void setGroupCriteria(GroupCriterionCollection value)
```


एक GroupCriteria संग्रह सेट करता है जो समूह परिभाषा में फ़ील्ड्स को दर्शाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) | एक GroupCriteria संग्रह जो समूह परिभाषा में फ़ील्ड्स को दर्शाता है। |

### setMaintainHierarchy(boolean value) {#setMaintainHierarchy-boolean-}
```
public final void setMaintainHierarchy(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के सारांश कार्य दिखाए जाएँ या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के सारांश कार्य दिखाए जाएँ या नहीं। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


एक Group ऑब्जेक्ट का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एक Group ऑब्जेक्ट का नाम। |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि प्रोजेक्ट रिबन में Group ड्रॉप-डाउन सूची में समूह का नाम दिखाता है या नहीं। |

### setShowSummary(boolean value) {#setShowSummary-boolean-}
```
public final void setShowSummary(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि समूह के लिए सारांश पंक्तियाँ प्रदर्शित की जाती हैं या नहीं। |

