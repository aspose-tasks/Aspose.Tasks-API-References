---
title: "ExtendedAttributeDefinition.CreateLookupResourceDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. طريقة مصنع تنشئ تعريف سمة موسعة مع بحث. لها CalculationType يساوي Lookup ويمكن استخدامها في Resources فقط. يُطلب منك تحديد fieldId و alias عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من field id"
type: docs
weight: 10
url: /ar/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

طريقة مصنع تنشئ تعريف سمة موسعة مع بحث. لها [`CalculationType`](../calculationtype/) يساوي Lookup ويمكن استخدامها في Resources فقط. يُطلب منك تحديد *fieldId* و *alias* عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من field id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | معرف الحقل المحدد لـ [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل مخصص لمورد مع بحث ثم ملئه بقيم نصية:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

طريقة مصنع تنشئ تعريف سمة موسعة مع بحث. لها [`CalculationType`](../calculationtype/) يساوي Lookup ويمكن استخدامها في Resources فقط. يُطلب منك تحديد *customFieldType* و *fieldId* و *alias* عند استدعاء هذه الطريقة.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| customFieldType | CustomFieldType | النوع المحدد لـ [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeResource | معرف الحقل المحدد لـ [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *customFieldType* و *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل مخصص لمورد مع بحث ثم ملئه بقيم نصية:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

يظهر كيفية إضافة سمات موسعة مع قوائم اختيار للتعيينات.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// تعيين المورد "1 TRG: Trade Group" إلى "TASK 1" بإنشاء كائن ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// إنشاء تعريف سمة مخصصة مع قائمة اختيار.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// يمكن رؤية هذه القيمة في عرض "Resource usage" في MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// إنشاء تعريف سمة مخصصة مع قائمة اختيار.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// يمكن رؤية هذه القيمة في عرض "Task usage" في MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// يمكن إزالة القيم الخاطئة لاحقًا.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// العمل مع المشروع...
```

### انظر أيضًا

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


