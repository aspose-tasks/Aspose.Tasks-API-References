---
title: "Task.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Genişletilmiş bir niteliğin değerlerini içeren ExtendedAttributeCollection nesnesini alır"
type: docs
weight: 400
url: /tr/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Genişletilmiş bir niteliğin değerlerini içeren ExtendedAttributeCollection nesnesini alır.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Açıklamalar

İki veri parçası gereklidir - benzersiz kimlik ya da Alan kimliği ile belirtilen uzatılmış nitelik tablosuna geri işaret eden bir gösterge ve değeri ya doğrudan değerle ya da değer listesine geri işaret eden bir gösterge.

## Örnekler

Görev genişletilmiş niteliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Genişletilmiş öznitelik tanımı oluştur
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Sıfır indeksli görevi al
var tsk = project.RootTask.Children.GetById(1);

// Genişletilmiş öznitelik ekle
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Ayrıca aşağıdaki kısa sözdizimi kullanılabilir: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Text1 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Bunu projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Öznitelik Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Oluşturulan Genişletilmiş Özniteliğe bir değer atayın. Öznitelik tipi "Text" olup, "TextValue" özelliği kullanılmalıdır.
taskExtendedAttributeText1.TextValue = "London";

// Genişletilmiş Özniteliği göreve ekleyin
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Text2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Bunu projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Id 1 için Text2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Genişletilmiş Özniteliği göreve ekleyin
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Duration2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Tanımı projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Id 3 için Duration2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Genişletilmiş Özniteliği göreve ekleyin
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Finish2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Tanımı projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Id 3 için Finish2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Genişletilmiş Özniteliği göreve ekleyin
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Görevler için genişletilmiş öznitelikleri okuyun
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

### Ayrıca Bakınız

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


