---
title: "Aspose::Tasks::Project::SetBaseline метод"
linktitle: "SetBaseline"
articleTitle: "SetBaseline"
second_title: "Aspose.Tasks для C++"
description: "Сохраняет поля базового плана в указанный базовый план для всего проекта."
type: docs
weight: 2060
url: /ru/cpp/aspose.tasks/project/setbaseline/
---

## SetBaseline (1 of 2) {#setbaseline_1}

Сохраняет поля базового плана в указанный базовый план для всего проекта.

**Returns:** void Aspose::Tasks::

```cpp
SetBaseline(BaselineType baselineType)
```

| Параметр | Описание |
| --- | --- |
| baselineType | Тип базовой линии для сохранения данных базовой линии. |

---

## SetBaseline (2 of 2) {#setbaseline_2}

Сохраняет поля базовой линии в указанную базовую линию для выбранных задач.

**Returns:** void Aspose::Tasks::

```cpp
SetBaseline(BaselineType baselineType, const System::SharedPtr< System::Collections::Generic::IEnumerable< System::SharedPtr< Task >>> & taskCollection)
```

| Параметр | Описание |
| --- | --- |
| baselineType | Тип базовой линии для сохранения данных базовой линии. |
| taskCollection | Список задач, для которых сохраняются данные базовой линии. |

