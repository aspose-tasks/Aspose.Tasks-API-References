---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraXmlSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα αποθηκευτεί μια ριζική εργασία ή όχι"
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα αποθηκευτεί μια ριζική εργασία ή όχι.

```csharp
public bool SaveRootTask { get; set; }
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


