---
title: "Κλάση CompoundDocumentHeaderException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.CompoundDocumentHeaderException κλάση. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν η κεφαλίδα του αρχείου MPP είναι κατεστραμμένη."
type: docs
weight: 280
url: /el/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν η κεφαλίδα του αρχείου MPP είναι κατεστραμμένη.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Παραδείγματα

Δείχνει πώς να πιάσετε την εξαίρεση &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


