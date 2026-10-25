---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कस्टम प्रोजेक्ट प्रॉपर्टीज़ का संग्रह दर्शाता है।"
type: docs
weight: 61
url: /hi/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

कस्टम प्रोजेक्ट प्रॉपर्टीज़ का संग्रह दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | नए [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | एक नई कस्टम प्रॉपर्टी बनाता है। |
| [add(String name, double value)](#add-java.lang.String-double-) | एक नई कस्टम प्रॉपर्टी बनाता है। |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | एक नई कस्टम प्रॉपर्टी बनाता है। |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | एक नई कस्टम प्रॉपर्टी बनाता है। |
| [clear()](#clear--) | PropertyCollection को साफ़ करता है। |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं; अन्यथा, false। |
| [remove(String name)](#remove-java.lang.String-) | संग्रह से निर्दिष्ट नाम वाली प्रॉपर्टी को हटाता है। |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


नए [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


एक नई कस्टम प्रॉपर्टी बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्रॉपर्टी का नाम। |
| मान | boolean | नव निर्मित प्रॉपर्टी ऑब्जेक्ट का मान। |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


एक नई कस्टम प्रॉपर्टी बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्रॉपर्टी का नाम। |
| मान | double | नव निर्मित प्रॉपर्टी ऑब्जेक्ट का मान। |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


एक नई कस्टम प्रॉपर्टी बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्रॉपर्टी का नाम। |
| मान | java.lang.String | नव निर्मित प्रॉपर्टी ऑब्जेक्ट का मान। |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


एक नई कस्टम प्रॉपर्टी बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्रॉपर्टी का नाम। |
| मान | java.util.Date | नव निर्मित प्रॉपर्टी ऑब्जेक्ट का मान। |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


PropertyCollection को साफ़ करता है।

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं; अन्यथा, false।

**Returns:**
boolean - यह दर्शाने वाला मान कि यह संग्रह केवल-पढ़ने योग्य है; अन्यथा, false।
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


संग्रह से निर्दिष्ट नाम वाली प्रॉपर्टी को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्रॉपर्टी का केस-इंसेंसिटिव नाम। |

**Returns:**
boolean - True यदि तत्व सफलतापूर्वक पाया गया और हटाया गया; अन्यथा false।
