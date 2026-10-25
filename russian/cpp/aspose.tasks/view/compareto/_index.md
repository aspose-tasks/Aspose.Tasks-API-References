---
title: "Aspose::Tasks::View::CompareTo метод"
linktitle: "CompareTo"
articleTitle: "CompareTo"
second_title: "Aspose.Tasks для C++"
description: "Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует ли за ним или находится"
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/view/compareto/
---

## CompareTo {#compareto}

Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует за ним или находится в том же положении в порядке сортировки, что и другой объект.

**Returns:** A 32-bit signed integer that indicates the relative order of the objects being compared. The return value has these meanings: Value Meaning Less than zero This instance precedes other in the sort order. Zero This instance occurs in the same position in the sort order as other . Greater than zero This instance follows other in the sort order.

```cpp
CompareTo(System::SharedPtr< View > other)
```

| Параметр | Описание |
| --- | --- |
| другой | у указанного объекта View, с которым сравнивается данный экземпляр. |

