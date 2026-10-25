---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yöntemi. Uid, görev adı, kaynak adı, iş ve süre atama sütunlarını içerir"
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Uid, görev adı, kaynak adı, iş ve süre atama sütunlarını içerir.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Dönüş Değeri

[`AssignmentViewColumn`](../../assignmentviewcolumn/) listesini içeren bir görünüm

## Örnekler

Atama görünümüyle bir projenin nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Ayrıca Bakınız

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


