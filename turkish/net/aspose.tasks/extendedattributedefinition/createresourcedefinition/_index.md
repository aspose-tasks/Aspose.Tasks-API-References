---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. Microsoft Project'in \"None\" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. CalculationType değeri None'dir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken customFieldType, fieldId ve alias belirtmeniz gerekir."
type: docs
weight: 30
url: /tr/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) değeri None'dir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen [`CustomFieldType`](../../customfieldtype/) türü. |
| fieldId | ExtendedAttributeResource | Belirtilen [`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *customFieldType*, *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Bu örneği kullanarak özel bir metin alanı tanımı oluşturun:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Bir kaynak atamasına genişletilmiş öznitelik eklemeyi gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Yeni görev ve kaynak ekle
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // "Resource Usage" görünümünde görünen özel öznitelikler, ExtendedAttributeDefinition.CreateResourceDefinition yöntemiyle oluşturulabilir.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Özniteliğin türü "Cost" olduğundan, "NumericValue" özelliğini kullanmamız gerekir.
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // "Task Usage" görünümünde görünen özel öznitelikler, ExtendedAttributeDefinition.CreateTaskDefinition yöntemiyle oluşturulabilir.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Özniteliğin türü "Cost" olduğundan, "NumericValue" özelliğini kullanmamız gerekir.
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) değeri None'dir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü, alan kimliğinden türetilir.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Belirtilen [`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Bu örneği kullanarak özel bir metin alanı tanımı oluşturun:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve bir bayrağın değerinin oluşturulurken nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// boolean özel alan için bir tanım oluştur.
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// bir öznitelik oluştur ve başlangıç değerini 'true' olarak ayarla.
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Ayrıca Bakınız

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


