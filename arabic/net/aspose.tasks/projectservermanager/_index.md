---
title: "الفئة ProjectServerManager"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.ProjectServerManager. الفئة التي توفر الطرق لقراءة وتنفيذ العمليات على المشاريع في حساب Project Online المحدد أو في مثيل Project Server المحلي المحدد. تدعم إصدارات Project Server 2016 و 2019."
type: docs
weight: 1500
url: /ar/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

الفئة التي توفر الطرق لقراءة وتنفيذ العمليات على المشاريع في حساب Project Online المحدد أو في مثيل Project Server المحلي المحدد (تُدعم إصدارات Project Server 2016 و2019).

```csharp
public sealed class ProjectServerManager
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | يُهيّئ مثيلاً جديداً من الفئة `ProjectServerManager`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | ينشئ مشروعًا جديدًا في مثيل Project Server\\Project Online باستخدام خيارات الحفظ الافتراضية. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | ينشئ مشروعًا جديدًا في نسخة Project Server\Project Online باستخدام خيارات الحفظ المحددة. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | يحصل على المشروع بالمعرف الفريد المحدد من حساب Project Online \ نسخة Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | يحصل على قائمة المشاريع من مخزن 'Working' لحساب Project Online الحالي \ نسخة Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | يحدّث المشروع الموجود في نسخة Project Server\Project Online باستخدام خيارات الحفظ الافتراضية. سيتم استبدال المشروع الموجود. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | يحدّث المشروع الموجود في نسخة Project Server\Project Online باستخدام خيارات الحفظ المحددة. سيتم استبدال المشروع الموجود. |

## الأحداث

| الاسم | الوصف |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | حدث يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات الويب الخاصة بـ Project Server. |

## الأمثلة

يوضح كيفية استخدام مدير Project Server لإنشاء مشروع جديد مع خيارات حفظ مسبقة التعريف على Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


