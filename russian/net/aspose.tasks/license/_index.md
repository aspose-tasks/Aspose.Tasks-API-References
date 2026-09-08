---
title: "Класс License"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.License. Предоставляет методы лицензирования компонента"
type: docs
weight: 980
url: /ru/net/aspose.tasks/license/
---
## License class

Предоставляет методы для лицензирования компонента.

```csharp
public sealed class License
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [License](license/)() | Инициализирует новый экземпляр класса `License`. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Лицензирует компонент. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Лицензирует компонент. |

## Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей компонент, в папке, содержащей вызывающую сборку, в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

файл jar компонента:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Показывает, как применить лицензию Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


