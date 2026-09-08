---
title: "LoadOptions.Password"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство LoadOptions. Получает или задает пароль защиты."
type: docs
weight: 50
url: /ru/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Получает или задает пароль защиты.

```csharp
public string Password { get; set; }
```

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

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


