---
title: "Класс InvalidPasswordException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.InvalidPasswordException. Представляет тип исключения, которое выбрасывается при открытии защищённого паролем файла с неверным паролем."
type: docs
weight: 910
url: /ru/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Представляет тип исключения, которое бросается при открытии защищённого паролем файла с неверным паролем.

```csharp
public class InvalidPasswordException : TasksException
```

## Примеры

Показывает, как обрабатывать &lt;see cref="InvalidPasswordException"/&gt; при чтении файлов проекта, защищённых паролем.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // работа с проектом ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // сообщение: "The project is password protected. The password is not provided or incorrect."
    Console.WriteLine(e.Message);
}
```

### См. также

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


