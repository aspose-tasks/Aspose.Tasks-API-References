---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "LoadOptions-Eigenschaft. Gibt die zum Einlesen eines Projekts aus den Formaten HTML, MPX, XER und Primavera XML verwendete Kodierung zurück oder legt sie fest. Die Standardkodierung ist UTF8."
type: docs
weight: 30
url: /de/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Gibt die zum Einlesen eines Projekts aus den Formaten HTML, MPX, XER und Primavera XML verwendete Kodierung zurück oder legt sie fest. Die Standardkodierung ist UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Beispiele

Zeigt, wie die Kodierung beim Öffnen eines Projekts aus einer Primavera‑XER‑Datei angegeben wird.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


