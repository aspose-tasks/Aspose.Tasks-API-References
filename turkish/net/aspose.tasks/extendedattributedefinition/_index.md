---
title: Class ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.ExtendedAttributeDefinition sınıf. Bir projeyle ilişkili genişletilmiş öznitelik tanımını temsil eder.
type: docs
weight: 540
url: /tr/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Bir projeyle ilişkili genişletilmiş öznitelik tanımını temsil eder.

```csharp
public class ExtendedAttributeDefinition
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Özel bir alanın diğer adını alır veya ayarlar. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Bir projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmediğini gösteren bir değer alır veya ayarlar. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Otomatik aşağı atamaların etkinleştirilip etkinleştirilmediğini gösteren bir değer alır veya ayarlar. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Özel özniteliğin değerinin hesaplama türünü alır veya ayarlar. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Özel alanın türünü alır. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Listedeki varsayılan değeri alır veya ayarlar. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Varsayılan arama tablosu girişinin Kılavuzunu alır veya ayarlar. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Bir görev, kaynak veya atamayla ilişkili genişletilmiş özniteliği alır veya ayarlar. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Alır veya ayarlar, özel bir alanın proje kimliğine karşılık gelir. Bir sabitin dize gösterimini kullanın[`ExtendedAttributeTask`](../extendedattributetask/) belirtmek için sınıf[`FieldId`](./fieldid/) özellik. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Özel bir alanın adını alır. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır veya ayarlar. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Özel bir alanın Kılavuzunu alır veya ayarlar. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Özel bir alanla ilişkili arama tablosunun bir Kılavuzunu alır. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Seçim listesinde ayarlayabileceğiniz maksimum değer sayısını alır veya ayarlar. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | için ana projeyi alır.`ExtendedAttributeDefinition` örnek. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Özel bir alanın takma adının fonetik telaffuzunu alır veya ayarlar. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Özel alan değerlerinin aşağıdaki değerlerle sınırlı olup olmadığını gösteren bir değer alır veya ayarlar:[`ValueList`](./valuelist/) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Toplamların hesaplanma şeklini alır veya ayarlar. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Genişletilmiş özniteliğin ikincil kılavuzunu alır veya ayarlar. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Özel bir alanın ikincil PID'sini alır veya ayarlar. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Özet satırları için özel öznitelik değerinin hesaplama türünü alır veya ayarlar. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Özel bir alanın kullanıcı tanımlı olup olmadığını gösteren bir değer alır veya ayarlar. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | &lt;Değer&gt; ValueList Listesini Alır. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Değer listelerinin sıralanma şeklini alır veya ayarlar. Değerler: 0=Azalan, 1=Artan. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](./calculationtype/) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](./calculationtype/) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](./calculationtype/) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](./calculationtype/) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntemi çağırırken. Alan türü, id. alanından çıkarılır. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype/) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırırken. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Dahili arama listesine bir değer ekler. Bu, manipülasyonlar için tercih edilen bir yoldur.[`ValueList`](./valuelist/) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Bu nesnenin alan kimliği değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Bu nesnenin alan kimliği değerine ve belirtilen bayrak değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Bu nesnenin alan kimliği değerine ve belirtilen tarih değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Bu nesnenin alan kimliği değerine ve belirtilen sayısal değere eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Bu nesnenin alan kimliği değerine ve belirtilen süre değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Bu nesnenin alan kimliği değerine ve belirtilen metin değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Belirtilen ile bağlantılı yeni genişletilmiş öznitelik oluşturur[`Value`](../value/) öğe. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Örneği için bir karma kod döndürür`ExtendedAttributeDefinition` sınıf. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Dahili arama listesinden bir değeri kaldırır. Bu, manipülasyonlar için tercih edilen bir yoldur.[`ValueList`](./valuelist/) . |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


