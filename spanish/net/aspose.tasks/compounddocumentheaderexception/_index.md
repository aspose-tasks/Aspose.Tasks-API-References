---
title: "Clase CompoundDocumentHeaderException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.CompoundDocumentHeaderException. Representa una excepción que se lanza cuando el encabezado del archivo MPP está dañado."
type: docs
weight: 280
url: /es/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Representa una excepción que se lanza cuando el encabezado del archivo MPP está dañado.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Ejemplos

Muestra cómo capturar la excepción &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


