---
title: "Task.OutlineCodes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает или задает объект OutlineCodeCollection"
type: docs
weight: 880
url: /ru/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Получает или задает объект [`OutlineCodeCollection`](../../outlinecodecollection/).

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Примечания

Необходимо два элемента данных — указатель на таблицу контурных кодов, указанную через FieldID, и значение, указанное либо через ValueID, либо через указатель ValueGUID к списку значений.

## Примеры

Показать, как прочитать значения outline code задачи.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### См. также

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


