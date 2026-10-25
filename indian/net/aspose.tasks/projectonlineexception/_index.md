---
title: "क्लास ProjectOnlineException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectOnlineException क्लास। जब Project Online या Project Server इंस्टेंस के साथ इंटरैक्शन के दौरान त्रुटियाँ मिलती हैं तो यह अपवाद फेंका जाता है।"
type: docs
weight: 1480
url: /hi/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

प्रोजेक्ट ऑनलाइन या प्रोजेक्ट सर्वर इंस्टेंस के साथ इंटरैक्शन के दौरान त्रुटियों मिलने पर फेंकी जाने वाली अपवाद को दर्शाता है।

```csharp
public class ProjectOnlineException : TasksException
```

## उदाहरण

MS Project Online से परियोजना पढ़ते समय अपवाद को कैसे पकड़ें, यह दिखाता है।

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


