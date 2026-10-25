---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. طريقة مصنع تنشئ تعريف سمة موسعة بسيط يظهر في Microsoft Project كـ None. لها CalculationType يساوي None ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد customFieldType و fieldId و alias عند استدعاء هذه الطريقة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

طريقة مصنع تنشئ تعريف سمة موسعة بسيط، يظهر في Microsoft Project كـ "None". لها [`CalculationType`](../calculationtype/) يساوي None ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد *customFieldType* و *fieldId* و *alias* عند استدعاء هذه الطريقة.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| customFieldType | CustomFieldType | النوع المحدد لـ [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeTask | معرف الحقل المحدد لـ [`ExtendedAttributeTask`](../../extendedattributetask/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *customFieldType* و *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

يوضح كيفية إنشاء السمات الموسعة للمهمة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// إنشاء تعريف سمة موسعة من النوع Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// أضفه إلى مجموعة Extended Attributes للمشروع
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// أضف مهمة إلى المشروع
var task = project.RootTask.Children.Add("Task 1");

// إنشاء سمة موسعة من تعريف Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// قم بتعيين قيمة للسمة الموسعة المُنشأة. نوع السمة هو "Text"، ويجب استخدام الخاصية "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// أضف Extended Attribute إلى المهمة
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// إنشاء تعريف سمة موسعة من النوع Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// إضافة قيم بحث لتعريف السمة الموسعة
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// أضفه إلى مجموعة Extended Attributes للمشروع
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// أضف مهمة إلى المشروع
var task2 = project4.RootTask.Children.Add("Task 2");

// إنشاء سمة موسعة من تعريف Text2 Lookup للمعرف 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// أضف Extended Attribute إلى المهمة
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// إنشاء تعريف سمة موسعة من النوع Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// أضف قيم البحث لتعريف السمة الموسعة
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// أضف التعريف إلى مجموعة Extended Attributes للمشروع
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// أضف مهمة إلى المشروع
var task3 = project2.RootTask.Children.Add("Task 3");

// إنشاء سمة موسعة من تعريف البحث Duration2 للمعرف 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// أضف Extended Attribute إلى المهمة
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// إنشاء تعريف سمة موسعة من النوع Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// أضف قيم البحث لتعريف السمة الموسعة
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// أضف التعريف إلى مجموعة Extended Attributes للمشروع
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// أضف مهمة إلى المشروع
var task4 = project3.RootTask.Children.Add("Task 4");

// إنشاء سمة موسعة من تعريف البحث Finish2 للمعرف 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// أضف Extended Attribute إلى المهمة
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، والذي يعرضه Microsoft Project كـ "None". يحتوي على [`CalculationType`](../calculationtype/) يساوي None ويمكن استخدامه في المهام فقط. يُطلب منك تحديد *fieldId* و *alias* عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من معرف الحقل.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | معرف الحقل المحدد لـ [`ExtendedAttributeTask`](../../extendedattributetask/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

يظهر كيفية إنشاء تعريف سمة موسعة وتعيين قيمة نصية للخاصية أثناء إنشائها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// إنشاء سمة موسعة بقيمة تساوي 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// إضافة سمة موسعة مبدئية بالقيمة 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### انظر أيضًا

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


