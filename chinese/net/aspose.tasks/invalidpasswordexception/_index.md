---
title: "类 InvalidPasswordException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.InvalidPasswordException 类。表示在使用错误密码打开受密码保护的文件时抛出的异常类型。"
type: docs
weight: 910
url: /zh/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

表示在使用错误密码打开受密码保护的文件时抛出的异常类型。

```csharp
public class InvalidPasswordException : TasksException
```

## 示例

展示如何在读取受密码保护的项目文件时处理 &lt;see cref="InvalidPasswordException"/&gt;。

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // 处理项目 …
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // 消息为 "项目受密码保护。未提供密码或密码不正确。"
    Console.WriteLine(e.Message);
}
```

### 另见

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


