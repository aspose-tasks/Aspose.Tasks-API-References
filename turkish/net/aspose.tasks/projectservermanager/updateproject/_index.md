---
title: ProjectServerManager.UpdateProject
second_title: Aspose.Tasks for .NET API Referansı
description: ProjectServerManager yöntem. Varsayılan kaydetme seçeneklerini kullanarak Project ServerProject Online örneğindeki mevcut projeyi günceller. Mevcut projenin üzerine yazılacak.
type: docs
weight: 70
url: /tr/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Varsayılan kaydetme seçeneklerini kullanarak Project Server\Project Online örneğindeki mevcut projeyi günceller. Mevcut projenin üzerine yazılacak.

```csharp
public void UpdateProject(Project project)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| project | Project | Project Server\Project Online örneğine kaydedilecek proje. |

### istisnalar

| istisna | şart |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya bir sunucu tarafından döndürülen hata durumunda. |

### Notlar

Proje özelliği 'project.Get(Prj.Guid)', Project Server hesabı \ Project Online örneğinde bulunan bir projenin geçerli bir kılavuzu olmalıdır.

### Örnekler

Bu örnekte, proje Project Online hesabından yüklenir, değiştirilir ve Project Online hesabına geri kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

### Ayrıca bakınız

* class [Project](../../project/)
* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Belirtilen kaydetme seçeneklerini kullanarak Project Server\Project Online örneğindeki mevcut projeyi günceller. Mevcut projenin üzerine yazılacak.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| project | Project | Project Server\Project Online örneğine kaydedilecek proje. |
| saveOptions | ProjectServerSaveOptions | Örneği[`ProjectServerSaveOptions`](../../projectserversaveoptions/) sınıf. |

### istisnalar

| istisna | şart |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya bir sunucu tarafından döndürülen hata durumunda. |

### Notlar

saveOptions.ProjectGuid, Project Server\ Project Online örneğinde bulunan bir projenin kılavuzuna ayarlanmalıdır.

### Örnekler

Bu örnekte, proje Project Online hesabından yüklenir, değiştirilir ve Project Online hesabına geri kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
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

### Ayrıca bakınız

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)


