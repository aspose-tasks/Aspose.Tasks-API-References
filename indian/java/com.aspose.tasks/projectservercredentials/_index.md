---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Project Online या ऑन-प्रेमाइस Project Server इंस्टेंस से कनेक्ट होने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स।"
type: docs
weight: 225
url: /hi/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Project Online या ऑन-प्रेमाइस Project Server इंस्टेंस से कनेक्ट होने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | SharePoint साइट के URL और SharePoint के PWA (Project Web Access) साइट के लिए वैध SPOIDCRL प्राधिकरण टोकन का उपयोग करके [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) क्लास का नया उदाहरण प्रारंभ करता है। |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | SharePoint साइट के URL, उपयोगकर्ता नाम और पासवर्ड का उपयोग करके [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) क्लास का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | SharePoint उदाहरण के लिए प्राधिकरण टोकन प्राप्त करता है। |
| [getSiteUrl()](#getSiteUrl--) | SharePoint साइट पर PWA का URL या ऑन-प्रेमाइज़ प्रोजेक्ट सर्वर का URL प्राप्त करता है। |
| [getUserName()](#getUserName--) | SharePoint साइट के लिए उपयोगकर्ता नाम प्राप्त करता है। |
| [toString()](#toString--) | इस उदाहरण का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


SharePoint साइट के URL और SharePoint के PWA (Project Web Access) साइट के लिए वैध SPOIDCRL प्राधिकरण टोकन का उपयोग करके [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online के PWA (Project Web Access) API का URL। |
|  | authToken | java.lang.String | SharePoint के PWA (Project Web Access) साइट के लिए प्राधिकरण टोकन (SPOIDCRL)। |

--------------------

जब आपके पास SharePoint Online साइट के लिए AuthToken पहले से हो, तो ProjectOnline से कनेक्ट करने के लिए इस कंस्ट्रक्टर का उपयोग करें। |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


SharePoint साइट के URL, उपयोगकर्ता नाम और पासवर्ड का उपयोग करके [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online के PWA (Project Web Access) API का URL। |
| userName | java.lang.String | SharePoint साइट के लिए उपयोगकर्ता नाम। |
|  | password | java.lang.String | SharePoint साइट के लिए पासवर्ड। |

--------------------

ProjectOnline से कनेक्ट करने के लिए इस कंस्ट्रक्टर का उपयोग करें। कृपया ध्यान दें कि लेगेसी प्रमाणीकरण आपके Azure पोर्टल और Office 365 एडमिन सेंटर में सक्षम होना चाहिए। |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


SharePoint उदाहरण के लिए प्राधिकरण टोकन प्राप्त करता है।

**Returns:**
java.lang.String - SharePoint उदाहरण के लिए प्राधिकरण टोकन।
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


SharePoint साइट पर PWA का URL या ऑन-प्रेमाइज़ प्रोजेक्ट सर्वर का URL प्राप्त करता है। उदाहरण के लिए, https://your\\_company\\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - SharePoint साइट पर PWA का URL या ऑन-प्रेमाइज़ प्रोजेक्ट सर्वर का URL।
### getUserName() {#getUserName--}
```
public final String getUserName()
```


SharePoint साइट के लिए उपयोगकर्ता नाम प्राप्त करता है।

**Returns:**
java.lang.String - SharePoint साइट के लिए उपयोगकर्ता नाम।
### toString() {#toString--}
```
public String toString()
```


इस उदाहरण का स्ट्रिंग प्रतिनिधित्व लौटाता है।

**Returns:**
java.lang.String - इस उदाहरण का स्ट्रिंग प्रतिनिधित्व।
