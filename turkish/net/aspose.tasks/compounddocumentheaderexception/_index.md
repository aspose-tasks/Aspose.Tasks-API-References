---
title: "Sınıf CompoundDocumentHeaderException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CompoundDocumentHeaderException sınıfı. MPP dosyasının başlığı bozulduğunda atılan bir istisna temsil eder"
type: docs
weight: 280
url: /tr/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

MPP dosyasının başlığı bozulduğunda atılan bir istisnayı temsil eder.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Örnekler

Nasıl &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; istisnasını yakalanacağını gösterir.

```csharp
try
{
    var project = new Project(DataDir + "Project1.mpp");

    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (CompoundDocumentHeaderException e)
{
    Console.WriteLine(e.Message);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


