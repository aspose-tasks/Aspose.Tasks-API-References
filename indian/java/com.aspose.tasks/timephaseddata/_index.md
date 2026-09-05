---
title: "TimephasedData"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "समय-फ़ेज़्ड डेटा का प्रतिनिधित्व करता है।"
type: docs
weight: 320
url: /hi/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

समय-फ़ेज़्ड डेटा का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | नया इंस्टेंस इनिशियलाइज़ करता है [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | लागत-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है। |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | लागत-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है। |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | सामग्री संसाधन के असाइनमेंट के यूनिट-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है। |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | कार्य-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है। |
| [getFinish()](#getFinish--) | समय‑फेज़्ड डेटा अवधि की समाप्ति तिथि प्राप्त करता है। |
| [getStart()](#getStart--) | समय‑फेज़्ड डेटा अवधि की प्रारंभ तिथि प्राप्त करता है। |
| [getTimephasedDataType()](#getTimephasedDataType--) | समय‑फेज़्ड डेटा का प्रकार प्राप्त करता है। |
| [getUid()](#getUid--) | समय‑फेज़्ड डेटा की अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [getUnit()](#getUnit--) | समय‑फेज़्ड डेटा अवधि की समय इकाई प्राप्त करता है। |
| [getValue()](#getValue--) | समय‑फेज़्ड डेटा अवधि के लिए प्रति समय इकाई मान प्राप्त करता है। |
| [getValueToCost()](#getValueToCost--) | `double` इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है। |
| [getValueToDuration()](#getValueToDuration--) | डबल इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है। |
| [getValueToUnits()](#getValueToUnits--) | `double` इंस्टेंस प्राप्त करता है जो यूनिट-आधारित समय‑फेज़्ड डेटा के लिए इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है। |
| [setFinish(Date value)](#setFinish-java.util.Date-) | समय‑फेज़्ड डेटा अवधि की समाप्ति तिथि सेट करता है। |
| [setStart(Date value)](#setStart-java.util.Date-) | समय‑फेज़्ड डेटा अवधि की प्रारंभ तिथि सेट करता है। |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | समय‑फेज़्ड डेटा का प्रकार सेट करता है। |
| [setUid(int value)](#setUid-int-) | समय‑फेज़्ड डेटा की अद्वितीय पहचानकर्ता सेट करता है। |
| [setUnit(byte value)](#setUnit-byte-) | समय‑फेज़्ड डेटा अवधि की समय इकाई सेट करता है। |
| [setValue(String value)](#setValue-java.lang.String-) | समय‑फेज़्ड डेटा अवधि के लिए प्रति समय इकाई मान सेट करता है। |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` इंस्टेंस जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है। |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


नया इंस्टेंस इनिशियलाइज़ करता है [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास का।

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


लागत-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | कार्य का UID। |
| प्रारंभ | java.util.Date | प्रारंभ तिथि‑समय। |
| समाप्ति | java.util.Date | समाप्ति तिथि‑समय। |
| मान | double | लागत मान। |
| प्रकार | byte | समय‑फेज़्ड डेटा प्रकार। |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


लागत-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | कार्य का UID। |
| प्रारंभ | java.util.Date | प्रारंभ तिथि‑समय। |
| समाप्ति | java.util.Date | समाप्ति तिथि‑समय। |
| मान | double | लागत मान। |
| समय इकाई | byte | समय इकाई प्रकार। |
| प्रकार | byte | समय‑फेज़्ड डेटा प्रकार। |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


सामग्री संसाधन के असाइनमेंट के यूनिट-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | कार्य का UID। |
| प्रारंभ | java.util.Date | प्रारंभ तिथि-समय। |
| समाप्ति | java.util.Date | समाप्ति तिथि‑समय। |
| इकाइयाँ | double | इकाइयों की संख्या। |
| प्रकार | byte | समय‑फेज़्ड डेटा प्रकार। |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


कार्य-आधारित समय‑फेज़्ड डेटा के लिए नई [TimephasedData](../../com.aspose.tasks/timephaseddata) क्लास की नई इंस्टेंस बनाता और प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | कार्य का UID। |
| प्रारंभ | java.util.Date | प्रारंभ तिथि‑समय। |
| समाप्ति | java.util.Date | समाप्ति तिथि‑समय। |
| मान | double | समय अंतराल मान। |
| समय इकाई | byte | समय इकाई प्रकार। |
| प्रकार | byte | समय‑फेज़्ड डेटा प्रकार। |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


समय‑फेज़्ड डेटा अवधि की समाप्ति तिथि प्राप्त करता है।

**Returns:**
java.util.Date - समय-चरणित डेटा अवधि की समाप्ति तिथि।
### getStart() {#getStart--}
```
public final Date getStart()
```


समय‑फेज़्ड डेटा अवधि की प्रारंभ तिथि प्राप्त करता है।

**Returns:**
java.util.Date - समय-चरणित डेटा अवधि की प्रारंभ तिथि।
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


समय‑फेज़्ड डेटा का प्रकार प्राप्त करता है।

--------------------

`Value`([getValue()](../../com.aspose/tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose/tasks/timephaseddata\#setValue-String-)) प्रॉपर्टी को साफ़ कर दिया जाएगा, यदि यह यहाँ निर्दिष्ट प्रकार के लिए उपयुक्त नहीं है।

**Returns:**
byte - समय-चरणित डेटा का प्रकार।
### getUid() {#getUid--}
```
public final int getUid()
```


समय‑फेज़्ड डेटा की अद्वितीय पहचानकर्ता प्राप्त करता है।

**Returns:**
int - समय-चरणित डेटा की विशिष्ट पहचानकर्ता।
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


समय‑फेज़्ड डेटा अवधि की समय इकाई प्राप्त करता है।

**Returns:**
byte - समय-चरणित डेटा अवधि की समय इकाई।
### getValue() {#getValue--}
```
public final String getValue()
```


समय‑फेज़्ड डेटा अवधि के लिए प्रति समय इकाई मान प्राप्त करता है।

**Returns:**
java.lang.String - समय-चरणित डेटा अवधि के लिए प्रति समय इकाई मान।
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


`double` इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है।

**Returns:**
double - वस्तु का फ्लोटिंग पॉइंट प्रतिनिधित्व।
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


डबल इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है।

**Returns:**
double - वस्तु का समय अंतराल प्रतिनिधित्व।
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


`double` इंस्टेंस प्राप्त करता है जो यूनिट-आधारित समय‑फेज़्ड डेटा के लिए इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है।

**Returns:**
double - इस वस्तु का फ्लोटिंग पॉइंट प्रतिनिधित्व।
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


समय‑फेज़्ड डेटा अवधि की समाप्ति तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | समय-चरणित डेटा अवधि की समाप्ति तिथि। |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


समय‑फेज़्ड डेटा अवधि की प्रारंभ तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | समय-चरणित डेटा अवधि की प्रारंभ तिथि। |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


समय‑फेज़्ड डेटा का प्रकार सेट करता है।

--------------------

`Value`([getValue()](../../com.aspose/tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose/tasks/timephaseddata\#setValue-String-)) प्रॉपर्टी को साफ़ कर दिया जाएगा, यदि यह यहाँ निर्दिष्ट प्रकार के लिए उपयुक्त नहीं है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | byte | समय-चरणित डेटा का प्रकार। |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


समय‑फेज़्ड डेटा की अद्वितीय पहचानकर्ता सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | समय-चरणित डेटा की विशिष्ट पहचानकर्ता। |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


समय‑फेज़्ड डेटा अवधि की समय इकाई सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | byte | समय-चरणित डेटा अवधि की समय इकाई। |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


समय‑फेज़्ड डेटा अवधि के लिए प्रति समय इकाई मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | समय-चरणित डेटा अवधि के लिए प्रति समय इकाई मान। |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` इंस्टेंस जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | `double` इंस्टेंस जो इस ऑब्जेक्ट के स्ट्रिंग मान का प्रतिनिधित्व करता है। |

