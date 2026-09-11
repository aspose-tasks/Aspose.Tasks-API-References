---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 350
url: /tr/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

MSP görünümünde görüntülenmek için görevlerin veya kaynakların karşılaması gereken kriterleri tanımlar.

FilterCriteria türü aşağıdaki üyeleri sunar:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| FilterCriteria() | FilterCriteria sınıfının yeni bir örneğini başlatır |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| işlem | Filtredeki diğer kriterlerle ilişkili olarak FieldName, Test ve Value ile belirlenen kriteri alır veya ayarlar. |
| field | Değiştirmek için bir [field](/tasks/python-net/aspose.tasks/filtercriteria/) alır veya ayarlar. |
| test | Filtre için seçim kriteri olarak işlev gören FieldName ve Value arasında yapılan karşılaştırma türünü alır veya ayarlar.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | FieldName ile belirtilen alanın değeriyle karşılaştırılacak nesne değerlerini alır. |
| criteria_rows | Alt [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) satırlarının listesini alır.<br/>            Filtre birden fazla kriter satırı içeriyorsa, And operatörünün etkisi, her iki satırın kriterlerinin de bu filtrenin sonucu olarak görev veya kaynağın gösterilmesi için karşılanması gerektiğidir.<br/>            Or operatörünün etkisi ise, satırlardan birinin kriterinin karşılanması gerektiğidir. |
## Methods
| Ad | Açıklama |
| :- | :- |
| is_field_value() | FilterCriteria'nin sağ taraftaki değerinin sabit bir değer değil, bir alan referansı olup olmadığını alır. |
| set_value_field(value) | Değeri FieldName ile belirtilen alanın değeriyle karşılaştırılacak alanı ayarlar. |

### Ayrıca Bakınız

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

