---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. ProjectDisplayOptions sınıfının bir örneğini alır"
type: docs
weight: 380
url: /tr/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

[`ProjectDisplayOptions`](../../projectdisplayoptions/) sınıfının bir örneğini alır.

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Örnekler

Projenin görüntüleme seçeneklerini nasıl ayarlayacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde uyarı gösterilip gösterilmeyeceğini belirten bir değeri ayarlar.
// Bu seçenek Project 2010 sürümü ve sonrasında kullanılabilir.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Ayrıca Bakınız

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


