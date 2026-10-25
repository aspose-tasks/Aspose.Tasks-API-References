---
title: "LoadOptions.Encoding"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété LoadOptions. Obtient ou définit l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. L'encodage par défaut est UTF8"
type: docs
weight: 30
url: /fr/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Obtient ou définit l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. L'encodage par défaut est UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Exemples

Montre comment spécifier l'encodage lors de l'ouverture d'un projet à partir d'un fichier Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


