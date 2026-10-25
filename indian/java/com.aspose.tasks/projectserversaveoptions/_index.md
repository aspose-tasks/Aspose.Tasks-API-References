---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट को Project Server या Project Online पर सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 227
url: /hi/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

प्रोजेक्ट को Project Server या Project Online पर सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) वर्ग का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | क्यू जॉब स्थिति अनुरोधों के बीच अंतराल प्राप्त करता है। |
| [getProjectGuid()](#getProjectGuid--) | परियोजना का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [getProjectName()](#getProjectName--) | परियोजना का नाम प्राप्त करता है जो Project Server \\ Project Online परियोजनाओं की सूची में प्रदर्शित होता है। |
| [getTimeout()](#getTimeout--) | Project Server की क्यू प्रोसेसिंग सेवा द्वारा सहेजें परियोजना अनुरोध की प्रक्रिया की प्रतीक्षा करते समय उपयोग किया जाने वाला टाइमआउट प्राप्त करता है। |
| [setPollingInterval(double value)](#setPollingInterval-double-) | क्यू जॉब स्थिति अनुरोधों के बीच अंतराल सेट करता है। |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | परियोजना का अद्वितीय पहचानकर्ता सेट करता है। |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | परियोजना का नाम सेट करता है जो Project Server \\ Project Online परियोजनाओं की सूची में प्रदर्शित होता है। |
| [setTimeout(double value)](#setTimeout-double-) | Project Server की क्यू प्रोसेसिंग सेवा द्वारा सहेजें परियोजना अनुरोध की प्रक्रिया की प्रतीक्षा करते समय उपयोग किया जाने वाला टाइमआउट सेट करता है। |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


[ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) वर्ग का नया उदाहरण प्रारंभ करता है।

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


क्यू जॉब स्थिति अनुरोधों के बीच अंतराल प्राप्त करता है। डिफ़ॉल्ट मान 2 सेकंड है।

**Returns:**
double - क्यू जॉब स्थिति अनुरोधों के बीच अंतराल।
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


परियोजना का अद्वितीय पहचानकर्ता प्राप्त करता है। यह Project Server \\ Project Online इंस्टेंस के भीतर अद्वितीय होना चाहिए।

**Returns:**
java.util.UUID - परियोजना का अद्वितीय पहचानकर्ता।
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


परियोजना का नाम प्राप्त करता है जो Project Server \\ Project Online परियोजनाओं की सूची में प्रदर्शित होता है। यह Project Server \\ Project Online इंस्टेंस के भीतर अद्वितीय होना चाहिए। यदि मान छोड़ा गया है, तो Prj.Name प्रॉपर्टी का मान उपयोग किया जाएगा।

**Returns:**
java.lang.String - Project Server \\ Project Online परियोजनाओं की सूची में प्रदर्शित होने वाला परियोजना नाम।
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Project Server की क्यू प्रोसेसिंग सेवा द्वारा सहेजें परियोजना अनुरोध की प्रक्रिया की प्रतीक्षा करते समय उपयोग किया जाने वाला टाइमआउट प्राप्त करता है। इस प्रॉपर्टी का डिफ़ॉल्ट मान 1 मिनट है।

--------------------

प्रोसेसिंग समय बड़े प्रोजेक्ट्स के लिए या जब प्रोजेक्ट सर्वर इंस्टेंस अन्य अनुरोधों का जवाब देने में बहुत व्यस्त हो, तो अधिक हो सकता है।

**Returns:**
double - टाइमआउट जिसका उपयोग प्रोजेक्ट सर्वर की क्यू प्रोसेसिंग सेवा द्वारा सहेजें प्रोजेक्ट अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय किया जाता है।
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


क्यू जॉब स्टेटस अनुरोधों के बीच अंतराल सेट करता है। डिफ़ॉल्ट मान 2 सेकंड है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | क्यू जॉब स्टेटस अनुरोधों के बीच अंतराल। |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


प्रोजेक्ट का यूनिक आइडेंटिफायर सेट करता है। यह प्रोजेक्ट सर्वर \ प्रोजेक्ट ऑनलाइन इंस्टेंस के भीतर यूनिक होना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.UUID | प्रोजेक्ट का यूनिक आइडेंटिफायर। |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


प्रोजेक्ट का नाम सेट करता है जो प्रोजेक्ट सर्वर \ प्रोजेक्ट ऑनलाइन प्रोजेक्ट सूची में दिखाया जाता है। यह प्रोजेक्ट सर्वर \ प्रोजेक्ट ऑनलाइन इंस्टेंस के भीतर यूनिक होना चाहिए। यदि मान छोड़ा गया है, तो Prj.Name प्रॉपर्टी का मान उपयोग किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | प्रोजेक्ट का नाम जो प्रोजेक्ट सर्वर \ प्रोजेक्ट ऑनलाइन प्रोजेक्ट सूची में दिखाया जाता है। |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


प्रोजेक्ट सर्वर की क्यू प्रोसेसिंग सेवा द्वारा सहेजें प्रोजेक्ट अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय उपयोग किया जाने वाला टाइमआउट सेट करता है। इस प्रॉपर्टी का डिफ़ॉल्ट मान 1 मिनट है।

--------------------

प्रोसेसिंग समय बड़े प्रोजेक्ट्स के लिए या जब प्रोजेक्ट सर्वर इंस्टेंस अन्य अनुरोधों का जवाब देने में बहुत व्यस्त हो, तो अधिक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | प्रोजेक्ट सर्वर की क्यू प्रोसेसिंग सेवा द्वारा सहेजें प्रोजेक्ट अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय उपयोग किया जाने वाला टाइमआउट। |

