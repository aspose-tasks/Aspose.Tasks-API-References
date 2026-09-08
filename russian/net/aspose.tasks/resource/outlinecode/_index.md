---
title: "Resource.OutlineCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Возвращает объект OutlineCodeCollection. Значение контурного кода"
type: docs
weight: 540
url: /ru/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Получает объект OutlineCodeCollection. Значение кода структуры.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Примечания

Необходимо два элемента данных — указатель на таблицу контурных кодов, указанную через FieldID, и значение, указанное либо через ValueID, либо через указатель ValueGUID к списку значений.

## Примеры

Показывает, как работать со значениями контуров ресурса.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### См. также

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


