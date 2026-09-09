---
title: "InvalidPasswordException sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.InvalidPasswordException sınıfı. Yanlış şifreyle şifre korumalı bir dosya açıldığında fırlatılan istisna türünü temsil eder."
type: docs
weight: 910
url: /tr/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Yanlış şifreyle şifre korumalı dosya açıldığında atılan istisna tipini temsil eder.

```csharp
public class InvalidPasswordException : TasksException
```

## Örnekler

Şifre korumalı proje dosyalarını okurken &lt;see cref="InvalidPasswordException"/&gt; nasıl ele alınacağını gösterir.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // projeyle çalışmak ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // mesaj şu şekildedir: "Proje şifre korumalıdır. Şifre sağlanmamış veya hatalıdır."
    Console.WriteLine(e.Message);
}
```

### Ayrıca Bakınız

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


