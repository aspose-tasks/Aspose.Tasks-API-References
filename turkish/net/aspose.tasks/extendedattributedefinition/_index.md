---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: Bir projeyle ilişkili genişletilmiş bir öznitelik tanımını temsil eder.
type: docs
weight: 530
url: /tr/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Bir projeyle ilişkili genişletilmiş bir öznitelik tanımını temsil eder.

```csharp
public class ExtendedAttributeDefinition
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Özel bir alanın diğer adını alır veya ayarlar. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Bir projeye eklenen yeni değerlerin listeye otomatik olarak eklenip eklenmediğini gösteren bir değer alır veya ayarlar. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Atamalara otomatik aşağı geçişin etkinleştirilip etkinleştirilmediğini gösteren bir değer alır veya ayarlar. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Özel özniteliğin değerinin hesaplama türünü alır veya ayarlar. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Özel alanın türünü alır. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Listedeki varsayılan değeri alır veya ayarlar. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Varsayılan arama tablosu girişinin Kılavuzunu alır veya ayarlar. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Bir görev, bir kaynak veya bir atama ile ilişkili genişletilmiş özniteliğini alır veya ayarlar. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Özel bir alanın proje kimliğine karşılık gelir veya ayarlar. [`ExtendedAttributeTask`](../extendedattributetask) belirtmek için sınıf[`FieldId`](./fieldid) özellik. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Özel bir alanın adını alır. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır veya ayarlar. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Özel bir alanın Kılavuzunu alır veya ayarlar. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Özel bir alanla ilişkili arama tablosunun Kılavuzunu alır. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Bir seçim listesinde ayarlayabileceğiniz maksimum değer sayısını alır veya ayarlar. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | için ana projeyi alır[`ExtendedAttributeDefinition`](../extendedattributedefinition) örnek. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Özel bir alanın diğer adının fonetik telaffuzunu alır veya ayarlar. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Özel alan değerlerinin aşağıdaki değerlerle sınırlı olup olmadığını gösteren bir değer alır veya ayarlar.[`ValueList`](./valuelist) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Toplamaların hesaplanma şeklini alır veya ayarlar. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Genişletilmiş özniteliğin ikincil kılavuzunu alır veya ayarlar. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Özel bir alanın ikincil PID'sini alır veya ayarlar. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Özet satırları için özel özniteliğin değerinin hesaplama türünü alır veya ayarlar. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Özel bir alanın kullanıcı tanımlı olup olmadığını gösteren bir değer alır veya ayarlar. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | &lt;Value&gt; ValueList. Listesini Alır |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Değer listelerinin sıralanma şeklini alır veya ayarlar. Değerler: 0=Azalan, 1=Artan. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Arama ile genişletilmiş bir öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekir*fieldId* ve*alias* bu yöntemi çağırdığınızda. Alan türü alan kimliğinden çıkarılır. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Arama ile genişletilmiş bir öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekir*customFieldType* ,*fieldId* ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Arama ile genişletilmiş bir öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*fieldId* ve*alias* bu yöntemi çağırdığınızda. Alan türü alan kimliğinden çıkarılır. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Arama ile genişletilmiş bir öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*customFieldType* ,*fieldId* ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekir*fieldId* ve*alias* bu yöntemi çağırdığınızda. Alan türü alan kimliğinden çıkarılır. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekir*customFieldType* ,*fieldId* ve*alias* bu yöntemi çağırdığınızda. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*fieldId* ve*alias* bu yöntemi çağırırken. Alan türü, alan kimliğinden çıkarılır. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](./calculationtype) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*customFieldType* ,*fieldId* ve*alias* bu yöntemi çağırırken. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Dahili arama listesine bir değer ekler. Bu, manipülasyonlar için tercih edilen bir yoldur.[`ValueList`](./valuelist) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Bu nesnenin alan kimliği değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Bu nesnenin alan kimliği değerine ve belirtilen bayrak değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Bu nesnenin alan kimliği değerine ve belirtilen tarih değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Bu nesnenin alan kimliği değerine ve belirtilen sayısal değere eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Bu nesnenin alan kimliği değerine ve belirtilen süre değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Bu nesnenin alan kimliği değerine ve belirtilen metin değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Belirtilenle bağlantılı yeni genişletilmiş öznitelik oluşturur[`Value`](../value) item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Örnek için bir karma kod döndürür[`ExtendedAttributeDefinition`](../extendedattributedefinition) sınıf. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Dahili arama listesinden bir değeri kaldırır. Bu, manipülasyonlar için tercih edilen bir yoldur.[`ValueList`](./valuelist) . |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
