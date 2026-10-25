---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerSaveOptions özelliği. Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesini beklerken kullanılan zaman aşımını alır veya ayarlar. Bu özelliğin varsayılan değeri 1 dakikadır."
type: docs
weight: 50
url: /tr/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesi beklenirken kullanılan zaman aşımını alır veya ayarlar. Bu özelliğin varsayılan değeri 1 dakikadır.

```csharp
public TimeSpan Timeout { get; set; }
```

## Açıklamalar

İşleme süresi, büyük projeler için veya Project Server örneği diğer isteklere yanıt vermekte çok meşgulse daha uzun olabilir.

## Örnekler

Microsoft Project Online'da projeyi nasıl güncelleyeceğinizi ve kaydetme zaman aşımı değerini nasıl kontrol edeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


