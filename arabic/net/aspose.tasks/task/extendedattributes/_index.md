---
title: "Task.ExtendedAttributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. يحصل على كائن ExtendedAttributeCollection يحتوي على قيم سمة موسعة"
type: docs
weight: 400
url: /ar/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

يحصل على كائن ExtendedAttributeCollection الذي يحتوي على قيم سمة موسعة.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## ملاحظات

هناك قطعتان من البيانات ضرورية - مؤشر يعود إلى جدول السمة الموسعة الذي يُحدَّد إما بالمعرّف الفريد أو معرف الحقل، والقيمة التي تُحدَّد إما بالقيمة نفسها أو بمؤشر يعود إلى قائمة القيم.

## الأمثلة

يعرض كيفية قراءة السمات الموسعة للمهمة.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// إنشاء تعريف سمة موسعة
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// احصل على مهمة الفهرس صفر
var tsk = project.RootTask.Children.GetById(1);

// إضافة سمة موسعة
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// يمكن أيضًا استخدام الصياغة المختصرة التالية: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// إنشاء تعريف سمة موسعة من النوع Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// أضفه إلى مجموعة Extended Attributes للمشروع
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// إنشاء سمة موسعة من تعريف Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// قم بتعيين قيمة للسمة الموسعة المُنشأة. نوع السمة هو "Text"، ويجب استخدام الخاصية "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// أضف Extended Attribute إلى المهمة
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// إنشاء تعريف سمة موسعة من النوع Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// إضافة قيم بحث لتعريف السمة الموسعة
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// أضفه إلى مجموعة Extended Attributes للمشروع
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// إنشاء سمة موسعة من تعريف Text2 Lookup للمعرف 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// أضف Extended Attribute إلى المهمة
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// إنشاء تعريف سمة موسعة من النوع Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// أضف قيم البحث لتعريف السمة الموسعة
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// أضف التعريف إلى مجموعة Extended Attributes للمشروع
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// إنشاء سمة موسعة من تعريف البحث Duration2 للمعرف 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// أضف Extended Attribute إلى المهمة
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// إنشاء تعريف سمة موسعة من النوع Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// أضف قيم البحث لتعريف السمة الموسعة
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// أضف التعريف إلى مجموعة Extended Attributes للمشروع
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// إنشاء سمة موسعة من تعريف البحث Finish2 للمعرف 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// أضف Extended Attribute إلى المهمة
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// قراءة السمات الموسعة للمهام
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


