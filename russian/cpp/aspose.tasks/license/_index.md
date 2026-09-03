---
title: "Aspose::Tasks::License класс"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks для C++"
description: "Предоставляет методы лицензирования компонента."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/license/
---

## License class

Предоставляет методы лицензирования компонента.

В этом примере будет выполнена попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей <ms> компонент, в папке, содержащей вызывающую сборку, в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> файл jar компонента:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Конструкторы

| Имя | Описание |
| --- | --- |
| [License](./license/) | Инициализирует новый экземпляр класса License. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Лицензирует компонент. |

