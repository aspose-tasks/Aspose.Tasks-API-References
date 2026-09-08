---
title: "LoadOptions.Encoding"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство LoadOptions. Получает или задает кодировку, используемую для чтения проекта из форматов HTML, MPX, XER и Primavera XML. Кодировка по умолчанию — UTF8."
type: docs
weight: 30
url: /ru/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Получает или задает кодировку, используемую для чтения проекта из форматов HTML, MPX, XER и Primavera XML. Кодировка по умолчанию — UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Примеры

Показывает, как указать кодировку при открытии проекта из файла Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


