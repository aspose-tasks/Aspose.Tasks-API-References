---
title: "الفئة InvalidPasswordException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.InvalidPasswordException. تمثل نوع الاستثناء الذي يُرمى عند فتح ملف محمي بكلمة مرور باستخدام كلمة مرور خاطئة"
type: docs
weight: 910
url: /ar/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

يمثل نوع الاستثناء الذي يُرمى عند فتح ملف محمي بكلمة مرور باستخدام كلمة مرور خاطئة.

```csharp
public class InvalidPasswordException : TasksException
```

## الأمثلة

يوضح كيفية التعامل مع &lt;see cref=\"InvalidPasswordException\"/&gt; أثناء قراءة ملفات مشروع محمية بكلمة مرور.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // العمل مع المشروع ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // الرسالة هي \"المشروع محمي بكلمة مرور. كلمة المرور غير مُقدمة أو غير صحيحة.\"
    Console.WriteLine(e.Message);
}
```

### انظر أيضًا

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


