---
title: "ExtendedAttributeDefinition sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ExtendedAttributeDefinition sınıfı. Bir proje ile ilişkili genişletilmiş öznitelik tanımını temsil eder."
type: docs
weight: 540
url: /tr/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Bir projeyle ilişkili genişletilmiş öznitelik tanımını temsil eder.

```csharp
public class ExtendedAttributeDefinition
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Özel alanın takma adını alır veya ayarlar. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Bir projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Atamalara otomatik olarak aşağı doğru yayılmanın etkin olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Özel öznitelik değerinin hesaplama türünü alır veya ayarlar. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Özel bir alanın türünü alır. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Listedeki varsayılan değeri alır veya ayarlar. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Varsayılan arama tablosu girdisinin Guid'ini alır veya ayarlar. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Genişletilmiş öznitelik bir görev, bir kaynak veya bir atama ile ilişkilendirilip ilişkilendirilmediğini alır veya ayarlar. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Özel bir alanın proje kimliğine karşılık gelen değeri alır veya ayarlar. [`ExtendedAttributeTask`](../extendedattributetask/) sınıfından bir sabitin dize temsilini kullanarak [`FieldId`](./fieldid/) özelliğini belirtin. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Özel bir alanın adını alır. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır veya ayarlar. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır veya ayarlar. MPP formatı için geçerlidir. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Özel bir alanın GUID'sini alır veya ayarlar. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Özel bir alanla ilişkili arama tablosunun GUID'sini alır. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Seçim listesinde ayarlayabileceğiniz maksimum değer sayısını alır veya ayarlar. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | `ExtendedAttributeDefinition` örneği için üst projeyi alır. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Özel bir alanın takma adının fonetik telaffuzunu alır veya ayarlar. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Özel alan değerlerinin [`ValueList`](./valuelist/) içindeki değerlerle sınırlı olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Toplamların nasıl hesaplandığını alır veya ayarlar. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Genişletilmiş özniteliğin ikincil GUID'sini alır veya ayarlar. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Özel bir alanın ikincil PID'sini alır veya ayarlar. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Özet satırlar için özel öznitelik değerinin hesaplama türünü alır veya ayarlar. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Özel bir alanın kullanıcı tanımlı olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | List&lt;Value&gt; ValueList'i alır. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Değer listelerinin nasıl sıralandığını alır veya ayarlar. Değerler: 0=Azalan, 1=Artan. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri Lookup'tir ve yalnızca Kaynaklarda kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri Lookup'tir ve yalnızca Kaynaklarda kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri Lookup'tir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri Lookup'tir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri None'dur ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri None'dur ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri None'dur ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) değeri None'dur ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | İç arama listesine bir değer ekler. Bu, [`ValueList`](./valuelist/) ile manipülasyonlar için tercih edilen bir yoldur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Bu nesnenin alan kimliği değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen bayrak değeriyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen tarih değeriyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen sayısal değerle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen süre değeriyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Bu nesnenin alan kimliği değerine eşit olan alan kimliği ve belirtilen metin değeriyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Belirtilen [`Value`](../value/) öğesiyle bağlantılı yeni bir genişletilmiş öznitelik oluşturur. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | `ExtendedAttributeDefinition` sınıfının örneği için bir karma kodu döndürür. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | İç arama listesinden bir değeri kaldırır. Bu, [`ValueList`](./valuelist/) ile manipülasyonlar için tercih edilen bir yoldur. |

## Örnekler

Genişletilmiş özniteliklerle ortak matematik fonksiyonlarının nasıl kullanılacağını gösterir.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Formülü Ayarla
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Genişletilmiş öznitelik değerini yazdır
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Formülü Ayarla
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Genişletilmiş öznitelik değerini yazdır
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Formülü Ayarla
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Genişletilmiş öznitelik değerini yazdır
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


