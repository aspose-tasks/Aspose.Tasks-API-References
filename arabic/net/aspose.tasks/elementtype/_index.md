---
title: "التعداد ElementType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.ElementType. يحدد نوع العنصر"
type: docs
weight: 490
url: /ar/net/aspose.tasks/elementtype/
---
## ElementType enumeration

يحدد نوع العنصر.

```csharp
public enum ElementType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Null | `0` | يشير إلى نوع العنصر Null. |
| Task | `1` | يشير إلى نوع العنصر Task. |
| Resource | `2` | يشير إلى نوع العنصر Resource. |
| Calendar | `3` | يشير إلى نوع العنصر Calendar. |
| Assignment | `4` | يشير إلى نوع العنصر Assignment. |

## الأمثلة

يوضح كيفية كتابة تعريفات السمات الموسعة المحدثة.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// إضافة سمة موسعة جديدة text3 مع بحث وقيمة بحث واحدة
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// إضافة سمة موسعة جديدة cost1 مع بحث وقيمتين للتكلفة
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// إضافة مهمة جديدة وتعيين قيمة بحث السمة.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// تعريف سمة مدة بدون بحث.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// إضافة مهمة جديدة وتعيين قيمة المدة إلى سمة المدة المعرفة مسبقًا.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


