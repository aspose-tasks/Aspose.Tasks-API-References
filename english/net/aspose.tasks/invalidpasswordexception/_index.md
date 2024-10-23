---
title: Class InvalidPasswordException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.InvalidPasswordException class. Represents the exception type which is thrown when password protected file opening with wrong password
type: docs
weight: 890
url: /net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Represents the exception type which is thrown when password protected file opening with wrong password.

```csharp
public class InvalidPasswordException : TasksException
```

## Examples

Shows how to handle &lt;see cref="InvalidPasswordException"/&gt; while reading a password protected project files.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // working with project ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // the message is "The project is password protected. The password is not provided or incorrect."
    Console.WriteLine(e.Message);
}
```

### See Also

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


