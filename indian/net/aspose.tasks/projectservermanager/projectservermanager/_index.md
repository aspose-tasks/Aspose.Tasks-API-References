---
title: ProjectServerManager
second_title: Aspose.Tasks for .NET API Reference
description: क एक नय उदहरण प्ररंभ करत हैProjectServerManageraspose.tasks/projectservermanager/ वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

का एक नया उदाहरण प्रारंभ करता है[`ProjectServerManager`](../) वर्ग.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| credentials | ProjectServerCredentials | प्रोजेक्ट ऑनलाइन खाते से कनेक्ट करने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स। |

### उदाहरण

यह उदाहरण दिखाता है कि प्रोजेक्ट सर्वर के ऑन-प्रिमाइसेस इंस्टेंस तक पहुँचने के लिए ProjectServerManager का इंस्टेंस कैसे बनाया जाए।

```csharp
[C#]
string site = "http:// project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

यह उदाहरण दिखाता है कि प्रोजेक्ट ऑनलाइन सेवा में खाते तक पहुँचने के लिए ProjectServerManager का उदाहरण कैसे बनाया जाए।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "पासवर्ड");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### यह सभी देखें

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* नाम स्थान [Aspose.Tasks](../../projectservermanager/)
* सभा [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
