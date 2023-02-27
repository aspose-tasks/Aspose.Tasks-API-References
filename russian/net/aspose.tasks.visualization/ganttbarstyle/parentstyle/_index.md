---
title: GanttBarStyle.ParentStyle
second_title: Справочник по Aspose.Tasks для .NET API
description: GanttBarStyle свойство. Получает или задает родительский или общий стиль для настраиваемого стиля для конкретной задачи.
type: docs
weight: 160
url: /ru/net/aspose.tasks.visualization/ganttbarstyle/parentstyle/
---
## GanttBarStyle.ParentStyle property

Получает или задает родительский (или общий) стиль для настраиваемого стиля для конкретной задачи.

```csharp
public GanttBarStyle ParentStyle { get; set; }
```

### Примечания

Задача может иметь несколько пользовательских стилей с разными родительскими стилями. Например, рассмотрим задачу, имеющую собственный стиль с родительским стилем «Критический» и другой стиль с родительским стилем «Обычный». Проще говоря, если задача является критической, применяется первый стиль. Если задача становится некритичной, применяется второй стиль (эта логика унаследована от Microsoft Project Professional).

### Смотрите также

* class [GanttBarStyle](../)
* пространство имен [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* сборка [Aspose.Tasks](../../../)


