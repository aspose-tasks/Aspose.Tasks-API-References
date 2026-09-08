---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraXmlSaveOptions. Получает или задает значение, указывающее, сохранять корневую задачу или нет"
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Получает или задаёт значение, указывающее, сохранять корневую задачу или нет.

```csharp
public bool SaveRootTask { get; set; }
```

## Примеры

Показывает, как экспортировать в файл Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### См. также

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


