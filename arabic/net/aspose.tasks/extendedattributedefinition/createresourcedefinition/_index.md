---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. طريقة مصنع تنشئ تعريف خاصية موسعة بسيط يظهر في Microsoft Project كـ None. لديها CalculationType مساوية لـ None ويمكن استخدامها في الموارد فقط. يجب عليك تحديد الحقول customFieldType و fieldId و alias عند استدعاء هذه الطريقة."
type: docs
weight: 30
url: /ar/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

طريقة مصنع تنشئ تعريف خاصية موسعة بسيط، يظهر في Microsoft Project كـ "None". لديها [`CalculationType`](../calculationtype/) مساوية لـ None ويمكن استخدامها في الموارد فقط. يُطلب منك تحديد *customFieldType* و *fieldId* و *alias* عند استدعاء هذه الطريقة.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| customFieldType | CustomFieldType | النوع المحدد لـ [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeResource | معرف الحقل المحدد لـ [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *customFieldType* و *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

يوضح كيفية إضافة خاصية موسعة إلى تعيين مورد.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// إضافة مهمة وموارد جديدة
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // يمكن إنشاء الخصائص المخصصة التي تظهر في عرض "Resource Usage" باستخدام طريقة ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // نوع الخاصية هو "Cost"، لذا نحتاج إلى استخدام خاصية "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // يمكن إنشاء الخصائص المخصصة التي تظهر في عرض "Task Usage" باستخدام طريقة ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // نوع الخاصية هو "Cost"، لذا نحتاج إلى استخدام خاصية "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

طريقة مصنع تنشئ تعريف خاصية موسعة بسيط، يظهر في Microsoft Project كـ "None". لديها [`CalculationType`](../calculationtype/) مساوية لـ None ويمكن استخدامها في الموارد فقط. يُطلب منك تحديد *fieldId* و *alias* عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من معرف الحقل.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | معرف الحقل المحدد لـ [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| الاسم المستعار | سلسلة | الاسم المستعار من نوع String المحدد. |

### قيمة الإرجاع

تم إنشاء نسخة من الفئة [`ExtendedAttributeDefinition`](../) مع *fieldId* و *alias* المحددين.

## الأمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


