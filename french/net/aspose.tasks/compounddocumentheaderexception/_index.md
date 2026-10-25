---
title: "Classe CompoundDocumentHeaderException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.CompoundDocumentHeaderException. Représente une exception qui est levée lorsque l’en-tête du fichier MPP est corrompu"
type: docs
weight: 280
url: /fr/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Représente une exception qui est levée lorsque l'en-tête du fichier MPP est corrompu.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Exemples

Montre comment attraper l’exception &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


