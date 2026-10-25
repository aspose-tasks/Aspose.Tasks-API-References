---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 310
url: /tr/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Bir projeyle ilişkili genişletilmiş öznitelik tanımını temsil eder.

ExtendedAttributeDefinition türü aşağıdaki üyeleri sunar:
## Özellikler
| Ad | Açıklama |
| :- | :- |
| field_id | Özel bir alanın proje kimliğine karşılık gelen değeri alır veya ayarlar.<br/>            Bu özelliği belirtmek için [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) sınıfındaki bir sabitin dize temsilini kullanın. |
| field_name | Özel bir alanın adını alır. |
| cf_type | Özel bir alanın türünü alır. |
| guid | Özel bir alanın GUID'ini alır veya ayarlar. |
| element_type | Genişletilmiş özelliğin bir görev, bir kaynak veya bir atama ile ilişkili olduğunu alır veya ayarlar.<br/>            bir görev, bir kaynak veya bir atama ile. |
| max_multi_values | Bir seçim listesinde ayarlayabileceğiniz maksimum değer sayısını alır veya ayarlar. |
| user_def | Özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını gösteren bir değeri alır veya ayarlar. |
| alias | Özel bir alanın takma adını alır veya ayarlar. |
| secondary_pid | Özel bir alanın ikincil PID'sini alır veya ayarlar. |
| auto_roll_down | Atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını gösteren bir değeri alır veya ayarlar. |
| default_guid | Varsayılan arama tablosu girişinin GUID'ini alır veya ayarlar. |
| lookup_uid | Özel bir alanla ilişkili arama tablosunun GUID'ini alır. |
| phonetics_alias | Özel bir alanın takma adının fonetik telaffuzunu alır veya ayarlar. |
| rollup_type | Toplamaların nasıl hesaplandığını alır veya ayarlar. |
| calculation_type | Özel özniteliğin değerinin hesaplama türünü alır veya ayarlar. |
| summary_rows_calculation_type | Özet satırlar için özel özniteliğin değerinin hesaplama türünü alır veya ayarlar. |
| formula | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır veya ayarlar. |
| graphical_indicator | Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır veya ayarlar.<br/>            MPP formatı için geçerlidir. |
| restrict_values | Özel alan değerlerinin [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) içindeki değerlerle sınırlı olup olmadığını gösteren bir değeri alır veya ayarlar. |
| valuelist_sort_order | Değer listelerinin sıralanma şeklini alır veya ayarlar. Değerler: 0=Azalan, 1=Artan. |
| append_new_values | Bir projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| default | Listedeki varsayılan değeri alır veya ayarlar. |
| value_list | ValueList adlı List<Value> öğesini alır. |
| secondary_guid | Genişletilmiş öznitelik için ikincil guid'i alır veya ayarlar. |
| parent_project | [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) örneği için üst proje nesnesini alır. |
## Methods
| Ad | Açıklama |
| :- | :- |
| create_extended_attribute() | Bu nesnenin alan kimliği değerine eşit alan kimliği ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(text_value) | Bu nesnenin alan kimliği değerine eşit alan kimliği ve belirtilen metin değeri ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(numeric_value) | Bu nesnenin alan kimliği değerine eşit alan kimliği ve belirtilen sayısal değer ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(date_time_value) | Bu nesnenin alan kimliği değerine eşit alan kimliği ve belirtilen tarih değeri ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(duration_value) | Bu nesnenin alan kimliği değerine eşit alan kimliği ve belirtilen süre değeri ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(flag_value) | Bu nesnenin alan kimliği değerine eşit alan kimliği ve belirtilen bayrak değeri ile yeni bir genişletilmiş öznitelik oluşturur. |
| create_extended_attribute(lookup_value) | Belirtilen [Value](/tasks/python-net/aspose.tasks/value/) öğesiyle bağlantılı yeni genişletilmiş öznitelik oluşturur. |
| create_task_definition(custom_field_type, field_id, alias) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [NONE](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_task_definition(field_id, alias) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [NONE](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_resource_definition(custom_field_type, field_id, alias) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [NONE](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Kaynakta kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_resource_definition(field_id, alias) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [NONE](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Kaynakta kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_lookup_task_definition(field_id, alias) | Arama (lookup) içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Arama (lookup) içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_lookup_resource_definition(field_id, alias) | Arama (lookup) içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Kaynaklarda kullanılabilir.<br/>            Belirtmeniz gerekir |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Arama (lookup) içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) değeri [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) olarak ayarlanmıştır ve yalnızca Kaynaklarda kullanılabilir.<br/>            Belirtmeniz gerekir |
| add_lookup_value(value) | İç arama listesine bir değer ekler. Bu, [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) ile manipülasyonlar için tercih edilen bir yoldur. |
| remove_lookup_value(value) | İç arama listesinden bir değeri kaldırır. Bu, [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) ile manipülasyonlar için tercih edilen bir yoldur. |

### Ayrıca Bakınız

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

