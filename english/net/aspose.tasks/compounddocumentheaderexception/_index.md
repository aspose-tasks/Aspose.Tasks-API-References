---
title: Class CompoundDocumentHeaderException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CompoundDocumentHeaderException class. Represents an exception which is thrown when the header of MPP file is broken
type: docs
weight: 280
url: /net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Represents an exception which is thrown when the header of MPP file is broken.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Examples

Shows how to catch &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; exception.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


