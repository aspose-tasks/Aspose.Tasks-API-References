---
title: "RiskPatternCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "RiskPattern वर्ग के उदाहरणों को सम्मिलित करने वाला एक संग्रह दर्शाता है।"
type: docs
weight: 269
url: /hi/java/com.aspose.tasks/riskpatterncollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class RiskPatternCollection extends AbstractCollection<RiskPattern>
```

`RiskPattern` क्लास के उदाहरणों को शामिल करने वाले संग्रह का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(RiskPattern item)](#add-com.aspose.tasks.RiskPattern-) | `RiskPattern` वर्ग का एक उदाहरण इस संग्रह में जोड़ता है। |
| [clear()](#clear--) | इस संग्रह से सभी आइटम हटाता है। |
| [contains(Object item)](#contains-java.lang.Object-) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [copyTo(RiskPattern[] array, int arrayIndex)](#copyTo-com.aspose.tasks.RiskPattern---int-) | इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर। |
| [get_Item(Task task)](#get-Item-com.aspose.tasks.Task-) | निर्दिष्ट कार्य के लिए `RiskPattern` वर्ग का उदाहरण प्राप्त करता है। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(Object item)](#remove-java.lang.Object-) | इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है। |
| [size()](#size--) | इस संग्रह में सम्मिलित तत्वों की संख्या लौटाता है। |
### add(RiskPattern item) {#add-com.aspose.tasks.RiskPattern-}
```
public boolean add(RiskPattern item)
```


`RiskPattern` वर्ग का एक उदाहरण इस संग्रह में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [RiskPattern](../../com.aspose.tasks/riskpattern) | इस संग्रह में जोड़ने के लिए `RiskPattern` वर्ग का एक उदाहरण। |

**Returns:**
boolean - यदि `RiskPattern` वर्ग का एक उदाहरण सफलतापूर्वक जोड़ा गया हो तो true लौटाता है; अन्यथा false।
### clear() {#clear--}
```
public void clear()
```


इस संग्रह से सभी आइटम हटाता है।

### contains(Object item) {#contains-java.lang.Object-}
```
public boolean contains(Object item)
```


यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | खोजने के लिए निर्दिष्ट आइटम। |

**Returns:**
बूलियन - यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true; अन्यथा false।
### copyTo(RiskPattern[] array, int arrayIndex) {#copyTo-com.aspose.tasks.RiskPattern---int-}
```
public void copyTo(RiskPattern[] array, int arrayIndex)
```


इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | [RiskPattern\[\]](../../com.aspose.tasks/riskpattern) | निर्दिष्ट एक-आयामी सरणी जिसमें तत्वों को कॉपी किया जाएगा। |
| arrayIndex | int | निर्दिष्ट एरे का शून्य-आधारित सूचकांक जहाँ प्रतिलिपि शुरू होती है। |

### get_Item(Task task) {#get-Item-com.aspose.tasks.Task-}
```
public RiskPattern get_Item(Task task)
```


निर्दिष्ट कार्य के लिए `RiskPattern` वर्ग का उदाहरण प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | निर्दिष्ट कार्य। |

**Returns:**
[RiskPattern](../../com.aspose.tasks/riskpattern) - the pattern for the specified task.
### iterator() {#iterator--}
```
public Iterator<RiskPattern> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskPattern&gt; - इस संग्रह के लिए एक इटेरेटर।
### remove(Object item) {#remove-java.lang.Object-}
```
public boolean remove(Object item)
```


इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | हटाने के लिए निर्दिष्ट वस्तु। |

**Returns:**
boolean - true यदि निर्दिष्ट वस्तु को इस संग्रह से सफलतापूर्वक हटा दिया गया हो; अन्यथा false।
### size() {#size--}
```
public int size()
```


इस संग्रह में सम्मिलित तत्वों की संख्या लौटाता है।

**Returns:**
int - इस संग्रह में शामिल तत्वों की संख्या।
