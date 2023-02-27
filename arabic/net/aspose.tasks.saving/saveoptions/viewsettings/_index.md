---
title: SaveOptions.ViewSettings
second_title: Aspose.Tasks لمرجع .NET API
description: SaveOptions ملكية. الحصول على عرض أو تعيينه View  لتقديمه. يمكنك استخدام هذه الخيارات لتحديد طريقة العرض التي يجب حفظها بتنسيق PDF أو HTML أو صورة بشكل صريح . إذا تم تعيين هذه الخاصية PresentationFormat يتم تجاهل الخاصية عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية Screen  Gantt  TaskSheet  TaskUsage  ResourceSheet  ResourceUsage
type: docs
weight: 240
url: /ar/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

الحصول على عرض أو تعيينه ([`View`](../view/) ) لتقديمه. يمكنك استخدام هذه الخيارات لتحديد طريقة العرض التي يجب حفظها بتنسيق PDF أو HTML أو صورة بشكل صريح . إذا تم تعيين هذه الخاصية ،[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) يتم تجاهل الخاصية عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية (([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt ، TaskSheet ، TaskUsage ، ResourceSheet ، ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | عندما يتم استدعاء طريقة التعيين ويتم توفير مثيل لفئة العرض مع قيمة غير مدعومة لخاصية الشاشة. |

### أنظر أيضا

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* مساحة الاسم [Aspose.Tasks.Saving](../../saveoptions/)
* المجسم [Aspose.Tasks](../../../)


