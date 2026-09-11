---
title: "TaskCollection"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 1140
url: /tr/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Bir [Task](/tasks/python-net/aspose.tasks/task/) nesnelerinden oluşan bir koleksiyonu temsil eder.

TaskCollection türü aşağıdaki üyeleri sunar:
## Özellikler
| Ad | Açıklama |
| :- | :- |
| ana_proje | TaskCollection nesnesinin üst proje nesnesini alır. |
## Methods
| Ad | Açıklama |
| :- | :- |
| add() | Belirtilen görevi [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) sınıfının örneğine ekleyin.<br/>            ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplayacaktır).<br/>            ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplayacaktır.<br/>            ParentProject.CalculationMode Automatic ise, yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır<br/>            (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar, gecikmeleri, iş ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar). |
| add(task_name) | Çocuk görevler koleksiyonuna yeni bir görev ekler. |
| add(task_name, before_task_id) |  |
| add(parameters) | Belirtilen kimliğe sahip bir görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler. |
| to_list() | TaskCollection nesnesini [Task](/tasks/python-net/aspose.tasks/task/) nesnelerinin bir listesine dönüştürür. |
| get_by_uid(uid) | Bu koleksiyonun üst görevi olan ve belirtilen Uid'ye sahip bir görevi döndürür. |
| get_by_id(id) | Bu koleksiyonun üst görevi olan ve belirtilen Id'ye sahip bir görevi döndürür. |

### Ayrıca Bakınız

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

