---
title: "Kelas CompoundDocumentHeaderException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.CompoundDocumentHeaderException. Mewakili pengecualian yang dilempar ketika header file MPP rusak"
type: docs
weight: 280
url: /id/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Mewakili pengecualian yang dilempar ketika header file MPP rusak.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Contoh

Menampilkan cara menangkap pengecualian &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

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

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


