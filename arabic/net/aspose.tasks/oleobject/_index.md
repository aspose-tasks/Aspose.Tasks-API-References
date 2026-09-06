---
title: "الفئة OleObject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.OleObject. تمثل كائن OLE يمكن إدراجه في عرض مخطط جانت لملف MPP"
type: docs
weight: 1120
url: /ar/net/aspose.tasks/oleobject/
---
## OleObject class

يمثل كائن OLE يمكن إدراجه في عرض مخطط Gantt لملف MPP.

```csharp
public class OleObject
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OleObject](oleobject/)() | يقوم بتهيئة نسخة جديدة من الفئة `OleObject`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | يحصل أو يضبط اسم التطبيق لفتح الكائن المضمّن به. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | يحصل أو يضبط بيانات الملف المضمّن؛ null إذا لم يتم تضمين أي بيانات. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | يحصل أو يضبط علامة تشير إلى أن كائن OLE يجب أن يُعرض إما كأيقونة أو كصورة عادية. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | يحصل أو يضبط تنسيق الملف للكائن المضمّن. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | يحصل أو يضبط المسار الكامل للكائن المُدرج. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | يحصل أو يضبط معرف الكائن. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | يحصل أو يضبط تسمية الكائن المُدرج. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | يحصل على قيمة تشير إلى ما إذا كان ملف المشروع يحتوي فقط على رابط للبيانات الفعلية المخزنة في مصدر الرابط. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | يحصل أو يضبط اسم نسخة كائن OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | يحصل أو يضبط المسار إلى الملف المؤقت للكائن المُدرج. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | يحصل أو يضبط نسخة الفئة [`View`](./view/) التي ينتمي إليها الكائن المُدرج. |

## الأمثلة

يعرض كيفية قراءة المعلومات حول كائنات OLE.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


