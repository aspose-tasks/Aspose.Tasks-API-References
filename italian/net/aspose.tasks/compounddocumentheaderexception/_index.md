---
title: "Classe CompoundDocumentHeaderException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.CompoundDocumentHeaderException. Rappresenta un'eccezione generata quando l'intestazione del file MPP è danneggiata."
type: docs
weight: 280
url: /it/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Rappresenta un'eccezione che viene lanciata quando l'intestazione del file MPP è danneggiata.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Esempi

Mostra come catturare l'eccezione &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


