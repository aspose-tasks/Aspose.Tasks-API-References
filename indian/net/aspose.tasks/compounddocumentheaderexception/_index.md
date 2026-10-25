---
title: "क्लास CompoundDocumentHeaderException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CompoundDocumentHeaderException क्लास। एक अपवाद का प्रतिनिधित्व करता है जो तब फेंका जाता है जब MPP फ़ाइल का हेडर टूट जाता है।"
type: docs
weight: 280
url: /hi/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

एक अपवाद का प्रतिनिधित्व करता है जो तब फेंका जाता है जब MPP फ़ाइल का हेडर टूट जाता है।

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## उदाहरण

कैसे &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; अपवाद को पकड़ें, दिखाता है।

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

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


