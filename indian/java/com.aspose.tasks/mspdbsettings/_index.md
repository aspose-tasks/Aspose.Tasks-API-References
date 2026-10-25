---
title: "MspDbSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "MS Project Server डेटाबेस से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।"
type: docs
weight: 161
url: /hi/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

MS Project Server डेटाबेस से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | नए उदाहरण को प्रारंभ करता है [MspDbSettings](../../com.aspose.tasks/mspdbsettings) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | पढ़ने के लिए प्रोजेक्ट का GUID प्राप्त करता है। |
| [getSchema()](#getSchema--) | MS Project Server का स्कीमा प्राप्त करता है। |
| [setSchema(String value)](#setSchema-java.lang.String-) | MS Project Server का स्कीमा सेट करता है। |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


नए उदाहरण को प्रारंभ करता है [MspDbSettings](../../com.aspose.tasks/mspdbsettings) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connectionString | java.lang.String | निर्दिष्ट कनेक्शन स्ट्रिंग। |
| projectGuid | java.util.UUID | पढ़ने के लिए प्रोजेक्ट का निर्दिष्ट GUID। |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


पढ़ने के लिए प्रोजेक्ट का GUID प्राप्त करता है।

**Returns:**
java.util.UUID - पढ़ने के लिए प्रोजेक्ट का GUID।
### getSchema() {#getSchema--}
```
public final String getSchema()
```


MS Project Server का स्कीमा प्राप्त करता है। डिफ़ॉल्ट मान "pub" है।

**Returns:**
java.lang.String - MS Project Server का स्कीमा।
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


MS Project Server का स्कीमा सेट करता है। डिफ़ॉल्ट मान "pub" है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | MS Project Server का स्कीमा। |

