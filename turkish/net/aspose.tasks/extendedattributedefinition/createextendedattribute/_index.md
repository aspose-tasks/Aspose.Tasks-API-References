---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. Bu nesnenin alan kimliği değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur"
type: docs
weight: 310
url: /tr/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Bu nesnenin alan kimliği değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

## Örnekler

Genişletilmiş özniteliklerin nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Custom alanı proje içinde yoksa, oluşturun.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Tanımdan Extended Attribute oluştur
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Göreve genişletilmiş öznitelik ekle
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen metin değeriyle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| textValue | Dize | Belirtilen metin değeri. |

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Mevcut [`CfType`](../cftype/) 'Text' değilse |

## Örnekler

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve öznitelik oluşturulurken bir dize değeri ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 'Common Info' değerine eşit bir genişletilmiş öznitelik oluştur
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// 'Common Info' değeriyle başlatılan genişletilmiş özniteliği ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen sayısal değerle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| numericValue | Decimal | Belirtilen sayısal değer. |

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Mevcut [`CfType`](../cftype/) 'Number' veya 'Cost' değilse |

## Örnekler

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve öznitelik oluşturulurken bir ondalık değer ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 999m değerine eşit bir genişletilmiş öznitelik oluştur
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// 999m değeriyle başlatılan genişletilmiş özniteliği ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen tarih değeriyle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTimeValue | DateTime | Belirtilen tarih saat değeri. |

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Eğer mevcut [`CfType`](../cftype/) 'Date', 'Start' veya 'Finish' değilse |

## Örnekler

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve öznitelik oluşturulurken tarih saat değerinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// Değeri DateTime.Now eşit olan genişletilmiş öznitelik oluştur
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// genişletilmiş öznitelik ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen süre değeriyle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| durationValue | Süre | Belirtilen süre değeri. |

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Eğer mevcut [`CfType`](../cftype/) 'Duration' değilse |

## Örnekler

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve oluşturulurken sürenin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// genişletilmiş öznitelik Duration1 = 2 gün
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// göreve genişletilmiş öznitelik ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen bayrak değeriyle yeni bir genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| flagValue | Boolean | Belirtilen bayrak değeri. |

### Dönüş Değeri

oluşturulan [`ExtendedAttribute`](../../extendedattribute/) sınıfının örneğini, bu nesnenin fieldID değerine eşit olan fieldID ile döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Eğer mevcut [`CfType`](../cftype/) 'Flag' değilse |

## Örnekler

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Belirtilen [`Value`](../../value/) öğesiyle bağlantılı yeni genişletilmiş öznitelik oluşturur.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| lookupValue | Value | Belirtilen [`Value`](../../value/) öğesi. |

### Dönüş Değeri

Belirtilen [`Value`](../../value/) öğesiyle bağlantılı [`ExtendedAttribute`](../../extendedattribute/) sınıfının oluşturulan örneğini döndürür.

## Açıklamalar

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Örnekler

Belirli bir değer kullanarak yeni [`ExtendedAttribute`](../../extendedattribute/) oluşturmak için bu kodu kullanın:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve oluşturulurken bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Yukarıda bildirilen arama tablosuna dayalı özel alan tanımı oluştur.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// bir değer için genişletilmiş öznitelik oluştur
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// göreve genişletilmiş öznitelik ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


