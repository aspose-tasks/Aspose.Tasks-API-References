---
title: "Класс LoadOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.LoadOptions. Позволяет указать дополнительные параметры загрузки при загрузке проекта из файла или потока."
type: docs
weight: 990
url: /ru/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Позволяет указать дополнительные параметры загрузки при загрузке проекта из файла или потока.

```csharp
public class LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LoadOptions](loadoptions/)() | Инициализирует новый экземпляр класса `LoadOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Получает или задает токен, который может использоваться для отмены операции загрузки проекта. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Получает или задает кодировку, используемую для чтения проекта из форматов HTML, MPX, XER и Primavera XML. Кодировка по умолчанию — UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Получает или задает метод обратного вызова для обработки ошибок разбора XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Получает или задает пароль защиты. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Получает или задает указанный экземпляр класса [`PrimaveraReadOptions`](../primaverareadoptions/), который может использоваться для настройки поведения загрузки форматов Primavera (Primavera P6 XER или Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Получает или задает обратный вызов, который будет вызываться во время операций загрузки проекта. В настоящее время поддерживается для форматов MPP и XER. |

## Примеры

Показывает, как загрузить проект, защищённый паролем, используя экземпляр &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


