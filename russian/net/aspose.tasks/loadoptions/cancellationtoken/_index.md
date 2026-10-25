---
title: "LoadOptions.CancellationToken"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство LoadOptions. Получает или задает токен, который может использоваться для отмены операции загрузки проекта."
type: docs
weight: 20
url: /ru/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Получает или задает токен, который может использоваться для отмены операции загрузки проекта.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примеры

Показывает, как передать CancellationToken для отмены длительной операции загрузки проекта.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts может быть передан в другой поток, где можно вызвать метод cts.Cancel() для отмены операции загрузки проекта.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


