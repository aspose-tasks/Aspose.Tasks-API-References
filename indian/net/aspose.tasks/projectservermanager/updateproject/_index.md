---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager मेथड। डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project ServerProject Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट कर दिया जाएगा।"
type: docs
weight: 70
url: /hi/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट किया जाएगा।

```csharp
public void UpdateProject(Project project)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | संचार त्रुटि या सर्वर द्वारा लौटाई गई त्रुटि की स्थिति में। |

## टिप्पणियाँ

प्रोजेक्ट की प्रॉपर्टी 'project.Get(Prj.Guid)' को एक वैध GUID होना चाहिए जो Project Server खाते \\ Project Online इंस्टेंस में मौजूद प्रोजेक्ट का हो।

## उदाहरण

इस उदाहरण में प्रोजेक्ट को Project Online खाते से लोड किया जाता है, संशोधित किया जाता है और फिर Project Online खाते में वापस सहेजा जाता है।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Microsoft Project Online पर प्रोजेक्ट को अपडेट करने का तरीका दर्शाता है।

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### संबंधित देखें

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट किया जाएगा।

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |
| saveOptions | ProjectServerSaveOptions | `ProjectServerSaveOptions` (../../projectserversaveoptions/) क्लास का इंस्टेंस। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | संचार त्रुटि या सर्वर द्वारा लौटाई गई त्रुटि की स्थिति में। |

## टिप्पणियाँ

saveOptions.ProjectGuid को उस प्रोजेक्ट के GUID पर सेट किया जाना चाहिए जो Project Server\\ Project Online इंस्टेंस में मौजूद है।

## उदाहरण

इस उदाहरण में प्रोजेक्ट को Project Online खाते से लोड किया जाता है, संशोधित किया जाता है और फिर Project Online खाते में वापस सहेजा जाता है।

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Project Server सहेजने विकल्पों के उपयोग के साथ Microsoft Project Online पर प्रोजेक्ट को अपडेट करने का तरीका दर्शाता है।

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### संबंधित देखें

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


