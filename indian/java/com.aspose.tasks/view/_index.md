---
title: "View"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट में एक दृश्य को दर्शाता है।"
type: docs
weight: 342
url: /hi/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

प्रोजेक्ट में एक दृश्य को दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [View()](#View--) | एक नया [View](../../com.aspose.tasks/view) वर्ग का उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | वर्तमान उदाहरण की तुलना समान प्रकार के दूसरे वस्तु से करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि वर्तमान उदाहरण क्रम में पहले आता है, बाद में, या दूसरे वस्तु के समान स्थिति में है। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | एक नया [View](../../com.aspose.tasks/view) वर्ग का उदाहरण बनाता है। |
| [getFilter()](#getFilter--) | एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को प्राप्त करता है। |
| [getGroup()](#getGroup--) | एकल दृश्य का समूह प्राप्त करता है। |
| [getHighlightFilter()](#getHighlightFilter--) | एकल दृश्य के लिए Microsoft Project फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getName()](#getName--) | एक View वस्तु का नाम प्राप्त करता है। |
| [getPageInfo()](#getPageInfo--) | `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) वर्ग का एक उदाहरण प्राप्त करता है। |
| [getParentProject()](#getParentProject--) | View वस्तु का पैरेंट प्राप्त करता है। |
| [getScreen()](#getScreen--) | एकल दृश्य के लिए स्क्रीन प्रकार प्राप्त करता है। |
| [getShowInMenu()](#getShowInMenu--) | Microsoft Project रिबन में View या Other Views ड्रॉप-डाउन सूची में एकल दृश्य का नाम दिखाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getTable()](#getTable--) | एकल दृश्य की तालिका प्राप्त करता है। |
| [getType()](#getType--) | एकल दृश्य में आइटम के प्रकार को प्राप्त करता है, जैसे कार्य या संसाधन। |
| [getUid()](#getUid--) | एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | दृश्य में [OleObject](../../com.aspose.tasks/oleobject) की स्थिति और रूप को दर्शाने वाले वस्तुओं का संग्रह प्राप्त करता है। |
| [hashCode()](#hashCode--) | इंस्टेंस के लिए हैश कोड मान लौटाता है [Resource](../../com.aspose.tasks/resource) क्लास का। |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को सेट करता है। |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | एकल दृश्य का समूह सेट करता है। |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | एकल दृश्य के लिए Microsoft Project फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setName(String value)](#setName-java.lang.String-) | एक View ऑब्जेक्ट का नाम सेट करता है। |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Microsoft Project रिबन में View या Other Views ड्रॉप‑डाउन सूची में एकल दृश्य का नाम दिखाता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | एकल दृश्य की तालिका सेट करता है। |
### View() {#View--}
```
public View()
```


एक नया [View](../../com.aspose.tasks/view) वर्ग का उदाहरण प्रारंभ करता है।

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


वर्तमान उदाहरण की तुलना समान प्रकार के दूसरे वस्तु से करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि वर्तमान उदाहरण क्रम में पहले आता है, बाद में, या दूसरे वस्तु के समान स्थिति में है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | इस उदाहरण की तुलना करने के लिए निर्दिष्ट View ऑब्जेक्ट। |

**Returns:**
int - एक 32‑बिट साइन्ड इंटीजर जो तुलना किए जा रहे वस्तुओं के सापेक्ष क्रम को दर्शाता है। रिटर्न मान के ये अर्थ हैं: मान अर्थ शून्य से कम यह उदाहरण `other` से पहले आता है। शून्य यह उदाहरण `other` के समान स्थिति में आता है। शून्य से अधिक यह उदाहरण `other` के बाद आता है।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
boolean - यदि निर्दिष्ट ऑब्जेक्ट एक View है जिसका Uid मान इस उदाहरण के समान है तो **True**; अन्यथा **false**।
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


एक नया [View](../../com.aspose.tasks/view) वर्ग का उदाहरण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| viewScreen | int | वह स्क्रीन प्रकार जिसके लिए दृश्य प्रदर्शित किया जा सकता है। |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को प्राप्त करता है।

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


एकल दृश्य का समूह प्राप्त करता है।

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


एकल दृश्य के लिए Microsoft Project फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि Microsoft Project एकल दृश्य के लिए फ़िल्टर को हाइलाइट करता है या नहीं।
### getName() {#getName--}
```
public final String getName()
```


एक View वस्तु का नाम प्राप्त करता है।

**Returns:**
java.lang.String - एक View ऑब्जेक्ट का नाम।
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


`PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) क्लास का एक उदाहरण प्राप्त करता है। यह mpp फ़ाइल प्रारूप में मौजूद पेज सेटअप डेटा का प्रतिनिधित्व करता है।

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View ऑब्जेक्ट का पैरेंट प्राप्त करता है। केवल‑पढ़ने योग्य [Project](../../com.aspose.tasks/project)।

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


एकल दृश्य के लिए स्क्रीन प्रकार प्राप्त करता है। केवल‑पढ़ने योग्य [ViewScreen](../../com.aspose.tasks/viewscreen)।

**Returns:**
int - एकल दृश्य के लिए स्क्रीन प्रकार।
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Microsoft Project रिबन में View या Other Views ड्रॉप-डाउन सूची में एकल दृश्य का नाम दिखाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि Microsoft Project रिबन में View या Other Views ड्रॉप‑डाउन सूची में एकल दृश्य का नाम दिखाता है या नहीं।
### getTable() {#getTable--}
```
public final Table getTable()
```


एकल दृश्य की तालिका प्राप्त करता है।

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


एकल दृश्य में आइटम के प्रकार को प्राप्त करता है, जैसे कार्य या संसाधन। केवल‑पढ़ने योग्य [ItemType](../../com.aspose.tasks/itemtype)।

**Returns:**
int - एकल दृश्य में आइटम का प्रकार, जैसे कार्य या संसाधन।
### getUid() {#getUid--}
```
public final int getUid()
```


एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है।

**Returns:**
int - एक दृश्य का अद्वितीय पहचानकर्ता।
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


दृश्य में [OleObject](../../com.aspose.tasks/oleobject) की स्थिति और रूप को दर्शाने वाले वस्तुओं का संग्रह प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - दृश्य में [OleObject](../../com.aspose.tasks/oleobject) की स्थिति और रूप को दर्शाने वाले वस्तुओं का संग्रह।
### hashCode() {#hashCode--}
```
public int hashCode()
```


इंस्टेंस के लिए हैश कोड मान लौटाता है [Resource](../../com.aspose.tasks/resource) क्लास का।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला दृश्य। |
| b | [View](../../com.aspose.tasks/view) | दूसरा दृश्य। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला दृश्य। |
| b | [View](../../com.aspose.tasks/view) | दूसरा दृश्य। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला दृश्य। |
| b | [View](../../com.aspose.tasks/view) | दूसरा दृश्य। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला दृश्य। |
| b | [View](../../com.aspose.tasks/view) | दूसरा दृश्य। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला फ़िल्टर। |
| b | [View](../../com.aspose.tasks/view) | दूसरा फ़िल्टर। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | पहला दृश्य। |
| b | [View](../../com.aspose.tasks/view) | दूसरा दृश्य। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | एकल दृश्य में उपयोग किया गया फ़िल्टर। |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


एकल दृश्य का समूह सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | एकल दृश्य का एक समूह। |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


एकल दृश्य के लिए Microsoft Project फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि Microsoft Project एकल दृश्य के लिए फ़िल्टर को हाइलाइट करता है या नहीं। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


एक View ऑब्जेक्ट का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एक View ऑब्जेक्ट का नाम। |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Microsoft Project रिबन में View या Other Views ड्रॉप‑डाउन सूची में एकल दृश्य का नाम दिखाता है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि Microsoft Project रिबन में View या Other Views ड्रॉप‑डाउन सूचियों में एकल दृश्य का नाम दिखाता है या नहीं। |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


एकल दृश्य की तालिका सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | एकल दृश्य की तालिका। |

