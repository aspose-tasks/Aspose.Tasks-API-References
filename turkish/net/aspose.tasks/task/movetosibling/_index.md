---
title: "Task.MoveToSibling"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Mevcut görevi aynı Taslak Seviyesinde belirtilen görevin önüne taşır. ParentProject.CalculationMode None ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate metodunu çağırmalıdır. Bu, tüm proje görevlerinin başlangıç/bitiş tarihlerini yeniden planlayacak, erken/geç tarihlerini ayarlayacak ve gecikmeler, iş ve maliyet alanları gibi bağımlı alanları taslak seviyeleriyle birlikte hesaplayacaktır. ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliği, taslak seviyesi ve taslak numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise, yöntem tüm proje görevlerini otomatik olarak yeniden planlayacak, başlangıç/bitiş tarihlerini ayarlayacak, erken/geç tarihlerini belirleyecek, gecikmeleri, işi ve maliyet alanlarını hesaplayacak, kimlikleri ve taslak seviyelerini yeniden hesaplayacaktır."
type: docs
weight: 1370
url: /tr/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Mevcut görevi aynı Outline Level'da, belirtilen görevin önüne taşır. ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, outline levels gibi bağımlı alanları hesaplayacaktır). ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini, Outline Level'i ve outline numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve Outline Level'leri yeniden hesaplar).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| beforeTask | Görev | Mevcut görevin ekleneceği görev. |

## Örnekler

Aynı üst görevin altında görevi nasıl taşıyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Kimliği 5 olan görevleri, kimliği 3 olan görevin önüne taşı.
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// VEYA
// Görevi koleksiyonun sonuna taşı.
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Mevcut görevi aynı Outline Level'da, belirtilen Id'ye sahip bir görevin önüne taşır. ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, outline levels gibi bağımlı alanları hesaplayacaktır). ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini, Outline Level'i ve outline numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve Outline Level'leri yeniden hesaplar).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| beforeTaskId | Int32 | Mevcut görevin ekleneceği görevin Id'si ([`Id`](../../tsk/id/)). |

## Örnekler

Görevin Id'sini kullanarak aynı üst görev altında görevi nasıl taşıyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Kimliği 5 olan görevleri, kimliği 3 olan görevin önüne taşı.
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// VEYA
// Görevi koleksiyonun sonuna taşı.
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


