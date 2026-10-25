---
title: "DbSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट डेटाबेस से पढ़ने के लिए सेटिंग्स निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 75
url: /hi/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

प्रोजेक्ट डेटाबेस से पढ़ने के लिए सेटिंग्स निर्दिष्ट करने की अनुमति देता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | कनेक्शन स्ट्रिंग प्राप्त करता है। |
| [getDriverClassName()](#getDriverClassName--) | JDBC ड्राइवर क्लास का नाम लौटाता है। |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | कनेक्शन स्ट्रिंग सेट करता है। |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | JDBC ड्राइवर क्लास का नाम सेट करता है। |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


कनेक्शन स्ट्रिंग प्राप्त करता है।

**Returns:**
java.lang.String - कनेक्शन स्ट्रिंग।
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


JDBC ड्राइवर क्लास का नाम लौटाता है। डिफ़ॉल्ट ड्राइवर क्लास नाम "com.microsoft.jdbc.sqlserver.SQLServerDriver" है।

**Returns:**
java.lang.String - ड्राइवर क्लास स्ट्रिंग।
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


कनेक्शन स्ट्रिंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कनेक्शन स्ट्रिंग। |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


JDBC ड्राइवर क्लास का नाम सेट करता है। डिफ़ॉल्ट ड्राइवर क्लास नाम "com.microsoft.jdbc.sqlserver.SQLServerDriver" है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | JDBC ड्राइवर क्लास का नाम। |

