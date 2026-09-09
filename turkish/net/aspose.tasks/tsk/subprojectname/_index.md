---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir alt projenin kaynak konumu"
type: docs
weight: 1070
url: /tr/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

Alt projenin kaynak konumu.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Örnekler

Alt proje görevi oluşturma nasıl yapılır gösterir.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Görev ekle
var task = project.RootTask.Children.Add("Task 1");

// Yeni alt proje bağlantısını ayarlama
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


