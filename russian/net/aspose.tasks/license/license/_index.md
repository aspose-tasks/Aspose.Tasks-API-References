---
title: "License.License"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор License. Инициализирует новый экземпляр класса License"
type: docs
weight: 10
url: /ru/net/aspose.tasks/license/license/
---
## License constructor

Инициализирует новый экземпляр класса [`License`](../).

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


