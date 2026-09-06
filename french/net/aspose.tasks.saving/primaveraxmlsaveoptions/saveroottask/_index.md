---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraXmlSaveOptions. Obtient ou définit une valeur indiquant s'il faut enregistrer une tâche racine ou non"
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Obtient ou définit une valeur indiquant s'il faut enregistrer une tâche racine ou non.

```csharp
public bool SaveRootTask { get; set; }
```

## Exemples

Montre comment exporter le fichier XML Primavera.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Voir aussi

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


