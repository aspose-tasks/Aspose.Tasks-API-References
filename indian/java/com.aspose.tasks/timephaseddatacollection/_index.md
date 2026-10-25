---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 321
url: /hi/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [TimephasedData](../../com.aspose.tasks/timephaseddata) वस्तुएँ होती हैं।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | नए उदाहरण को प्रारंभ करता है [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वर्ग का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | इस संग्रह वस्तु में [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरण जोड़ता है। |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | इस संग्रह वस्तु में [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरणों का संग्रह जोड़ता है। |
| [clear()](#clear--) | सभी आइटम हटाता है [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से। |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | निर्धारित करता है कि क्या [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) में कोई विशिष्ट मान है। |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | तत्वों को [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से एक Array में कॉपी करता है, एक विशेष Array सूचकांक से शुरू होकर। |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो संकेत देता है कि System.Collections.Generic.ICollection&lt;T&gt; केवल-पढ़ने योग्य है या नहीं। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक इटररेटर लौटाता है। |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | इस संग्रह वस्तु से [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरण हटाता है। |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | `startTime` और `finishTime` के बीच सभी समय चरणों का चयन करता है। |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | निर्दिष्ट अनुक्रमांक पर तत्व सेट करता है। |
| [size()](#size--) | इस [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वस्तु में सम्मिलित वस्तुओं की संख्या प्राप्त करता है। |
| [toList()](#toList--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वस्तु को [TimephasedData](../../com.aspose.tasks/timephaseddata) वस्तुओं की सूची में परिवर्तित करता है। |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


नए उदाहरण को प्रारंभ करता है [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वर्ग का।

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


इस संग्रह वस्तु में [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरण जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | जोड़ने के लिए आइटम। |

**Returns:**
boolean - true, यदि आइटम जोड़ा गया; अन्यथा false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


इस संग्रह वस्तु में [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरणों का संग्रह जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | जोड़ने के लिए [TimephasedData](../../com.aspose.tasks/timephaseddata) वस्तुओं का संग्रह। |

### clear() {#clear--}
```
public final void clear()
```


सभी आइटम हटाता है [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से।

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


निर्धारित करता है कि क्या [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) में कोई विशिष्ट मान है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | संग्रह में खोजने के लिए वस्तु। |

**Returns:**
boolean - true यदि `item` संग्रह में पाया जाता है; अन्यथा false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


तत्वों को [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से एक Array में कॉपी करता है, एक विशेष Array सूचकांक से शुरू होकर।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से कॉपी किए गए तत्वों का गंतव्य एक-आयामी Array है। Array में शून्य-आधारित अनुक्रमण होना चाहिए। |
| arrayIndex | int | `array` में शून्य-आधारित सूचकांक जहाँ कॉपी शुरू होती है। |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


एक मान प्राप्त करता है जो संकेत देता है कि System.Collections.Generic.ICollection&lt;T&gt; केवल-पढ़ने योग्य है या नहीं।

**Returns:**
boolean - यदि System.Collections.Generic.ICollection<T> केवल-पढ़ने योग्य है तो true; अन्यथा false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


इस संग्रह के लिए एक इटररेटर लौटाता है।

**Returns:**
java.util.Iterator<com.aspose.tasks.TimephasedData> - इस संग्रह के लिए एक इटररेटर।
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


इस संग्रह वस्तु से [TimephasedData](../../com.aspose.tasks/timephaseddata) उदाहरण हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | हटाने के लिए आइटम। |

**Returns:**
boolean - यदि `item` को सफलतापूर्वक [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) से हटाया गया हो तो true; अन्यथा false। यह मेथड भी false लौटाता है यदि `item` को [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) में नहीं पाया गया।
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


`startTime` और `finishTime` के बीच सभी टाइम फेज़ को चुनता है। औसत मामले में O(log n) जटिलता रखता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timephasedDataType | byte | चयन करने के लिए टाइम फेज़ का प्रकार। |
| startTime | java.util.Date | इंटरवल की शुरुआत। |
| finishTime | java.util.Date | इंटरवल का अंत। |

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) डेटा का नया सूची इंस्टेंस लौटाता है, जो Start प्रॉपर्टी द्वारा क्रमबद्ध है।
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


निर्दिष्ट अनुक्रमांक पर तत्व सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | सेट करने के लिए तत्व का शून्य-आधारित सूचकांक। |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | सेट करने के लिए तत्व। |

### size() {#size--}
```
public final int size()
```


इस [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वस्तु में सम्मिलित वस्तुओं की संख्या प्राप्त करता है।

**Returns:**
int - इस [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ऑब्जेक्ट में सम्मिलित वस्तुओं की संख्या।
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) वस्तु को [TimephasedData](../../com.aspose.tasks/timephaseddata) वस्तुओं की सूची में परिवर्तित करता है।

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - [TimephasedData](../../com.aspose.tasks/timephaseddata) वस्तुओं की सूची।
