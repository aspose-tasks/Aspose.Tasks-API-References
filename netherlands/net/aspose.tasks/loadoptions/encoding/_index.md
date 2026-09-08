---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LoadOptions-eigenschap. Haalt op of stelt de codering in die wordt gebruikt om een project te lezen uit HTML, MPX, XER- en Primavera XML-formaten. De standaardcodering is UTF8."
type: docs
weight: 30
url: /nl/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Haalt de codering op of stelt deze in die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. De standaardcodering is UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Voorbeelden

Toont hoe de codering kan worden gespecificeerd bij het openen van een project uit een Primavera XER-bestand.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Zie ook

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


