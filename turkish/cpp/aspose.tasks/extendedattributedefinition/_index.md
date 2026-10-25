---
title: "Aspose::Tasks::ExtendedAttributeDefinition sınıfı"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "C++ için Aspose.Tasks"
description: "Bir projeye bağlı genişletilmiş öznitelik tanımını temsil eder."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Bir projeye bağlı genişletilmiş öznitelik tanımını temsil eder.

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | İç arama listesine bir değer ekler. Bu, ValueList ile manipülasyonlar için tercih edilen bir yoldur. |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Bu nesnenin alan kimliği değerine eşit olan alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::Lookup'e eşittir ve yalnızca Kaynaklarda kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::Lookup'e eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::None'a eşittir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::None'a eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken customFieldType, fieldId ve alias belirtmeniz gerekir. |
| [Equals](./equals/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| [get_Alias](./get_alias/) | Özel bir alanın takma adını alır. |
| [get_AppendNewValues](./get_appendnewvalues/) | Bir projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmediğini gösteren bir değeri alır. |
| [get_AutoRollDown](./get_autorolldown/) | Atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını gösteren bir değeri alır. |
| [get_CalculationType](./get_calculationtype/) | Özel öznitelik değerinin hesaplama türünü alır. |
| [get_CfType](./get_cftype/) | Özel bir alanın tipini alır. |
| [get_Default](./get_default/) | Listede varsayılan değeri alır. |
| [get_DefaultGuid](./get_defaultguid/) | Varsayılan arama tablosu girişinin Guid'ini alır. |
| [get_ElementType](./get_elementtype/) | Genişletilmiş özniteliğin bir görev, bir kaynak veya bir atama ile ilişkili olduğunu alır. |
| [get_FieldId](./get_fieldid/) | Özel bir alanın proje kimliğine karşılık gelen değeri alır. FieldId özelliğini belirtmek için Aspose::Tasks::ExtendedAttributeTask sınıfındaki bir sabitin dize temsilini kullanın. |
| [get_FieldName](./get_fieldname/) | Özel bir alanın adını alır. |
| [get_Formula](./get_formula/) | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır. MPP formatı için geçerlidir. |
| [get_Guid](./get_guid/) | Özel bir alanın Guid'ini alır. |
| [get_LookupUid](./get_lookupuid/) | Özel bir alanla ilişkili arama tablosunun Guid'ini alır. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Seçim listesinde ayarlayabileceğiniz maksimum değer sayısını alır. |
| [get_ParentProject](./get_parentproject/) | ExtendedAttributeDefinition örneği için üst proje alınır. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Özel bir alanın takma adının fonetik telaffuzunu alır. |
| [get_RestrictValues](./get_restrictvalues/) | Özel alan değerlerinin ValueList'teki değerlerle sınırlı olup olmadığını gösteren bir değeri alır. |
| [get_RollupType](./get_rolluptype/) | Toplamaların nasıl hesaplandığını alır. |
| [get_SecondaryGuid](./get_secondaryguid/) | Genişletilmiş özniteliğin ikincil guid'ini alır. |
| [get_SecondaryPid](./get_secondarypid/) | Özel bir alanın ikincil PID'sini alır. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Özet satırlar için özel özniteliğin değerinin hesaplama tipini alır. |
| [get_UserDef](./get_userdef/) | Özel bir alanın kullanıcı tanımlı olup olmadığını gösteren bir değeri alır. |
| [get_ValueList](./get_valuelist/) | List< Value > ValueList'i alır. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Değer listelerinin nasıl sıralandığını alır. Değerler: 0=Azalan, 1=Artan. |
| [GetHashCode](./gethashcode/) | ExtendedAttributeDefinition sınıfının örneği için bir hash kodu döndürür. |
| [RemoveLookupValue](./removelookupvalue/) | Dahili arama listesinden bir değeri kaldırır. Bu, ValueList ile manipülasyonlar için tercih edilen bir yoldur. |
| [set_Alias](./set_alias/) | Özel bir alanın takma adını ayarlar. |
| [set_AppendNewValues](./set_appendnewvalues/) | Projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmeyeceğini gösteren bir değeri ayarlar. |
| [set_AutoRollDown](./set_autorolldown/) | Atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını belirten bir değer ayarlar. |
| [set_CalculationType](./set_calculationtype/) | Özel niteliğin değerinin hesaplama türünü ayarlar. |
| [set_Default](./set_default/) | Listede varsayılan değeri ayarlar. |
| [set_DefaultGuid](./set_defaultguid/) | Varsayılan arama tablosu girişinin Guid'ini ayarlar. |
| [set_ElementType](./set_elementtype/) | Genişletilmiş niteliğin bir görev, bir kaynak veya bir atama ile ilişkilendirilmesini ayarlar. |
| [set_FieldId](./set_fieldid/) | Özel alanın proje kimliğine karşılık gelen ayarı yapar. FieldId özelliğini belirtmek için Aspose::Tasks::ExtendedAttributeTask sınıfındaki bir sabitin dize temsilini kullanın. |
| [set_Formula](./set_formula/) | Microsoft Project'in özel görev alanını doldurmak için kullandığı formülü ayarlar. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Genişletilmiş nitelikle ilişkili grafik gösterge bilgilerini ayarlar. MPP formatı için geçerlidir. |
| [set_Guid](./set_guid/) | Özel bir alanın Guid'ini ayarlar. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Seçim listesinde ayarlayabileceğiniz maksimum değer sayısını ayarlar. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Özel bir alanın takma adının fonetik telaffuzunu ayarlar. |
| [set_RestrictValues](./set_restrictvalues/) | Özel alan değerlerinin ValueList'teki değerlerle sınırlı olup olmadığını belirten bir değer ayarlar. |
| [set_RollupType](./set_rolluptype/) | Toplamların nasıl hesaplandığını ayarlar. |
| [set_SecondaryGuid](./set_secondaryguid/) | Genişletilmiş niteliğin ikincil guid'ini ayarlar. |
| [set_SecondaryPid](./set_secondarypid/) | Özel bir alanın ikincil PID'sini ayarlar. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Özet satırlar için özel niteliğin değerinin hesaplama türünü ayarlar. |
| [set_UserDef](./set_userdef/) | Özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını belirten bir değer ayarlar. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Değer listelerinin sıralama şeklini ayarlar. Değerler: 0=Azalan, 1=Artan. |

