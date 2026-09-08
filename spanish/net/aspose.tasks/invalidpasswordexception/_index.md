---
title: "Clase InvalidPasswordException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.InvalidPasswordException. Representa el tipo de excepción que se lanza al abrir un archivo protegido con contraseña con una contraseña incorrecta."
type: docs
weight: 910
url: /es/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Representa el tipo de excepción que se lanza cuando se abre un archivo protegido con contraseña con una contraseña incorrecta.

```csharp
public class InvalidPasswordException : TasksException
```

## Ejemplos

Muestra cómo manejar &lt;see cref="InvalidPasswordException"/&gt; al leer archivos de proyecto protegidos con contraseña.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // trabajando con proyecto ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // el mensaje es "El proyecto está protegido con contraseña. La contraseña no se ha proporcionado o es incorrecta."
    Console.WriteLine(e.Message);
}
```

### Ver también

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


