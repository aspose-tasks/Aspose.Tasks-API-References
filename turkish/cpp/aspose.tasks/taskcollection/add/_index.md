---
title: "Aspose::Tasks::TaskCollection::Add metodu"
linktitle: "Ekle"
articleTitle: "Ekle"
second_title: "C++ için Aspose.Tasks"
description: "Yeni görevi, proje görevleri koleksiyonuna, son görevin aynı taslak seviyesinde ekler."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Yeni görevi, proje görevleri koleksiyonuna, son görevin aynı taslak seviyesinde ekler.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Belirtilen id'ye sahip bir görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parametre | Açıklama |
| --- | --- |
| parametreler | Tekrarlayan görev oluşturmak için belirtilen parametreler. |

---

## Add (3 of 5) {#add_3}

Belirtilen görevi TaskCollection sınıfının örneğine ekleyin. ParentProject.CalculationMode None ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihlerini, erken/son tarihleri ayarlar) yeniden zamanlar ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplar). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Automatic ise, yöntem tüm proje görevlerini otomatik olarak yeniden zamanlar (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar, gecikmeleri, iş ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parametre | Açıklama |
| --- | --- |
| öğe | Bu görev koleksiyonuna eklenmesi gereken belirtilen görev. |

---

## Add (4 of 5) {#add_4}

Alt görevler koleksiyonuna yeni bir görev ekler.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parametre | Açıklama |
| --- | --- |
| taskName | belirtilen görev adı. |

---

## Add (5 of 5) {#add_5}

Çocuk görevler koleksiyonuna yeni yinelenen bir görev ekler.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parametre | Açıklama |
| --- | --- |
| taskName | belirtilen görev adı. |
| beforeTaskId | Yeni bir görevin ekleneceği görevin öncesindeki belirtilen görev kimliği. |

