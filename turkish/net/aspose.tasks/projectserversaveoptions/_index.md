---
title: "Sınıf ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectServerSaveOptions sınıfı. Proje Project Server veya Project Online'a kaydedildiğinde ek seçenekler belirtmeye olanak tanır."
type: docs
weight: 1510
url: /tr/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Proje Project Server veya Project Online'a kaydedildiğinde ek seçenekler belirtmeye olanak tanır.

```csharp
public sealed class ProjectServerSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Yeni bir `ProjectServerSaveOptions` sınıfının örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Kuyruk iş durumu istekleri arasındaki aralığı alır veya ayarlar. Varsayılan değer 2 saniyedir. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Bir projenin benzersiz tanımlayıcısını alır veya ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adını alır veya ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır. Değer atlanırsa, Prj.Name özelliğinin değeri kullanılacaktır. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesi beklenirken kullanılan zaman aşımını alır veya ayarlar. Bu özelliğin varsayılan değeri 1 dakikadır. |

## Örnekler

Yerel (on-premise) Project Server örneğinde yeni bir proje oluşturmak için &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; seçeneklerinin nasıl kullanılacağını gösterir.

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
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


