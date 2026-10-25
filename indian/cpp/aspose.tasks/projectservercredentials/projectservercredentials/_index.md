---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials कंस्ट्रक्टर"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks C++ के लिए"
description: "SharePoint साइट के URL और वैध SPOIDCRL प्राधिकरण टोकन का उपयोग करके ProjectServerCredentials क्लास का नया इंस्टेंस इनिशियलाइज़ करता है (SharePoint की PWA (Proj"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

SharePoint साइट के URL और SharePoint के PWA (Project Web Access) साइट के लिए वैध SPOIDCRL प्राधिकरण टोकन का उपयोग करके ProjectServerCredentials क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| पैरामीटर | विवरण |
| --- | --- |
| siteUrl | Project Online की PWA (Project Web Access) API का URL। |
| authToken | SharePoint की PWA (Project Web Access) साइट के लिए प्राधिकरण टोकन (SPOIDCRL)। |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

SharePoint साइट के URL, उपयोगकर्ता नाम और पासवर्ड का उपयोग करके ProjectServerCredentials क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| पैरामीटर | विवरण |
| --- | --- |
| siteUrl | Project Online की PWA (Project Web Access) API का URL। |
| userName | SharePoint साइट के लिए उपयोगकर्ता नाम। |
| password | SharePoint साइट के लिए पासवर्ड। |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Project Web Access एंडपॉइंट के URL और नेटवर्क क्रेडेंशियल्स का उपयोग करके ProjectServerCredentials क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| पैरामीटर | विवरण |
| --- | --- |
| siteUrl | Project Web Access एंडपॉइंट का URL। |
| credentials | Project Web Access एंडपॉइंट में लॉगिन करने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स। |

