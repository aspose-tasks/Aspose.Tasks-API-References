---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager मेथड। डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server/Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है।

```csharp
public void CreateNewProject(Project project)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | संचार त्रुटि या सर्वर द्वारा लौटाई गई त्रुटि की स्थिति में। |

## उदाहरण

इस उदाहरण में प्रोजेक्ट को .mpp फ़ाइल से लोड किया जाता है और Project Online खाते में सहेजा जाता है।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

दिखाता है कि कैसे ProjectServerManager का उपयोग करके Microsoft Project Online पर नया प्रोजेक्ट बनाया जाए।

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है।

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |
| saveOptions | ProjectServerSaveOptions | `ProjectServerSaveOptions` (../../projectserversaveoptions/) क्लास का इंस्टेंस। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | संचार त्रुटि या सर्वर द्वारा लौटाई गई त्रुटि की स्थिति में। |

## उदाहरण

इस उदाहरण में प्रोजेक्ट को .mpp फ़ाइल से लोड किया जाता है और Project Online खाते में सहेजा जाता है।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

दिखाता है कि Microsoft Project Online पर पूर्वनिर्धारित सहेजने विकल्पों के साथ नया प्रोजेक्ट बनाने के लिए Project Server मैनेजर का उपयोग कैसे किया जाए।

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


