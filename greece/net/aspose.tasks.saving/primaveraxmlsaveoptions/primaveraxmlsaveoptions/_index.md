---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PrimaveraXmlSaveOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης PrimaveraXmlSaveOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraXmlSaveOptions`](../).

```csharp
public PrimaveraXmlSaveOptions()
```

## Παραδείγματα

Δείχνει πώς να εξάγετε στο αρχείο Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Δείτε επίσης

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


