---
title: ProjectServerManager.CreateNewProject
second_title: Aspose.Tasks for .NET API Referansı
description: ProjectServerManager yöntem. Varsayılan kaydetme seçeneklerini kullanarak Project ServerProject Online örneğinde yeni proje oluşturur.
type: docs
weight: 30
url: /tr/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Varsayılan kaydetme seçeneklerini kullanarak Project Server\Project Online örneğinde yeni proje oluşturur.

```csharp
public void CreateNewProject(Project project)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| project | Project | Project Server\Project Online örneğine kaydedilecek proje. |

### istisnalar

| istisna | şart |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya bir sunucu tarafından döndürülen hata durumunda. |

### Örnekler

Bu örnekte proje .mpp dosyasından yüklenir ve Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

### Ayrıca bakınız

* class [Project](../../project/)
* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Belirtilen kaydetme seçeneklerini kullanarak Project Server\Project Online örneğinde yeni proje oluşturur.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| project | Project | Project Server\Project Online örneğine kaydedilecek proje. |
| saveOptions | ProjectServerSaveOptions | Örneği[`ProjectServerSaveOptions`](../../projectserversaveoptions/) sınıf. |

### istisnalar

| istisna | şart |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya bir sunucu tarafından döndürülen hata durumunda. |

### Örnekler

Bu örnekte proje .mpp dosyasından yüklenir ve Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

### Ayrıca bakınız

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)


