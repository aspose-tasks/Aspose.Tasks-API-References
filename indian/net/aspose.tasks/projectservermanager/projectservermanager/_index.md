---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager कंस्ट्रक्टर। ProjectServerManager क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

`ProjectServerManager` (../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्रेडेंशियल्स | ProjectServerCredentials | Project Online खाते से कनेक्ट करने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स। |

## उदाहरण

यह उदाहरण दिखाता है कि कैसे ProjectServerManager का इंस्टेंस बनाकर ऑन-प्रिमाइस Project Server तक पहुंचा जाए।

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

यह उदाहरण दिखाता है कि कैसे ProjectServerManager का इंस्टेंस बनाकर Project Online सेवा में खाते तक पहुंचा जाए।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Microsoft Project Online से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### संबंधित देखें

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


