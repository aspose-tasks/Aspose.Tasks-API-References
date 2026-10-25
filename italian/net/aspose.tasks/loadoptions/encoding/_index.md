---
title: "LoadOptions.Encoding"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta la codifica utilizzata per leggere un progetto dai formati HTML, MPX, XER e Primavera XML. La codifica predefinita è UTF8"
type: docs
weight: 30
url: /it/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Ottiene o imposta la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. La codifica predefinita è UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Esempi

Mostra come specificare la codifica aprendo un progetto da un file Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


