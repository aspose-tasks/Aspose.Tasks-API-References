---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. تنشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن"
type: docs
weight: 310
url: /ar/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

## الأمثلة

يظهر كيفية إنشاء السمات الموسعة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// إذا لم يكن الحقل المخصص موجوداً في المشروع، قم بإنشائه.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// إنشاء سمة موسعة من التعريف
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// إضافة سمة موسعة إلى المهمة
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للنص.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| textValue | سلسلة | قيمة النص المحددة. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا كان [`CfType`](../cftype/) الحالي ليس 'Text' |

## الأمثلة

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة الرقمية المحددة.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| numericValue | Decimal | القيمة الرقمية المحددة. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا كان [`CfType`](../cftype/) الحالي ليس 'Number' أو 'Cost' |

## الأمثلة

يظهر كيفية إنشاء تعريف سمة موسعة وتعيين قيمة عشرية للخاصية أثناء إنشائها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// إنشاء سمة موسعة بقيمة تساوي 999m
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// إضافة سمة موسعة مبدئية بالقيمة 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للتاريخ.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dateTimeValue | DateTime | القيمة المحددة للوقت والتاريخ. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا كان [`CfType`](../cftype/) الحالي ليس 'Date' أو 'Start' أو 'Finish' |

## الأمثلة

يوضح كيفية إنشاء تعريف سمة ممتدة وتعيين قيمة تاريخ ووقت للسمة أثناء إنشائها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// إنشاء سمة ممتدة بقيمة تساوي DateTime.Now
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// إضافة سمة ممتدة
task.ExtendedAttributes.Add(extendedAttribute);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للمدة.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| durationValue | المدة | القيمة المحددة للمدة. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا كان [`CfType`](../cftype/) الحالي ليس 'Duration' |

## الأمثلة

يوضح كيفية إنشاء تعريف سمة ممتدة وتعيين مدة أثناء إنشائها.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// سمة ممتدة Duration1 = 2 أيام
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// إضافة سمة ممتدة إلى المهمة
task.ExtendedAttributes.Add(extendedAttribute);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

ينشئ سمة موسعة جديدة مع معرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للعلامة.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| flagValue | Boolean | القيمة المحددة للعلامة. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) مع fieldID الذي يساوي قيمة fieldID لهذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا كان [`CfType`](../cftype/) الحالي ليس 'Flag' |

## الأمثلة

يوضح كيفية إنشاء تعريف سمة موسعة وتعيين قيمة علم أثناء بنائه.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// إنشاء تعريف لحقل مخصص من نوع منطقي
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// إنشاء سمة وتعيين القيمة الأولية إلى 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

ينشئ سمة ممتدة جديدة مرتبطة بالعنصر [`Value`](../../value/) المحدد.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| lookupValue | Value | العنصر [`Value`](../../value/) المحدد. |

### قيمة الإرجاع

يعيد نسخة تم إنشاؤها من الفئة [`ExtendedAttribute`](../../extendedattribute/) المرتبطة بالعنصر [`Value`](../../value/) المحدد.

## ملاحظات

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## الأمثلة

استخدم هذا الكود لإنشاء [`ExtendedAttribute`](../../extendedattribute/) جديد باستخدام قيمة محددة:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

يوضح كيفية إنشاء تعريف سمة ممتدة وتعيين قيمة أثناء إنشائها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// إنشاء تعريف حقل مخصص بناءً على جدول البحث الذي تم إعلانه أعلاه.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// إنشاء سمة ممتدة لقيمة
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// إضافة سمة ممتدة إلى المهمة
task.ExtendedAttributes.Add(extendedAttribute);
```

### انظر أيضًا

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


