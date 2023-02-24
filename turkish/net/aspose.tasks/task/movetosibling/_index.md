---
title: Task.MoveToSibling
second_title: Aspose.Tasks for .NET API Referansı
description: Task yöntem. Geçerli görevi belirtilen görevden önceki aynı Anahat Düzeyine taşır. Eğer ParentProject.CalculationMode Yok ise kullanıcı bu yöntemi kullandıktan sonra Project.Recalculatei çağırmalıdır Tüm proje görevlerini başlangıç/bitiş tarihleri erken ayarlar yeniden planlar/ geç tarihler ve bolluklar çalışma ve maliyet alanları anahat seviyeleri gibi bağımlı alanları hesaplayın. ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini anahat seviyesini ve anahat numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Otomatik ise yöntem tüm proje görevlerini otomatik olarak yeniden planlar başlangıç/bitiş tarihleri erken/geç tarihleri ayarlar boşlukları iş ve maliyet alanlarını hesaplar kimlikleri ve anahat düzeylerini yeniden hesaplar.
type: docs
weight: 1370
url: /tr/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Geçerli görevi belirtilen görevden önceki aynı Anahat Düzeyine taşır. Eğer ParentProject.CalculationMode Yok ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate()'i çağırmalıdır (Tüm proje görevlerini (başlangıç/bitiş tarihleri, erken ayarlar) yeniden planlar/ geç tarihler) ve bolluklar, çalışma ve maliyet alanları, anahat seviyeleri gibi bağımlı alanları hesaplayın). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, anahat seviyesini ve anahat numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Otomatik ise yöntem tüm proje görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, boşlukları, iş ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| beforeTask | Task | Geçerli görevin önüne ekleneceği görev. |

### Ayrıca bakınız

* class [Task](../)
* ad alanı [Aspose.Tasks](../../task/)
* toplantı [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Geçerli görevi, belirtilen Id'ye sahip bir görevden önceki aynı Anahat Düzeyine taşır. ParentProject.CalculationMode Yok ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate()'i çağırmalıdır (Tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) ve bolluklar, çalışma ve maliyet alanları, anahat seviyeleri gibi bağımlı alanları hesaplar). CalculationMode Otomatiktir, yöntem tüm projenin görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, boşlukları, iş ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| beforeTaskId | Int32 | kimlik ([`Id`](../../tsk/id/)) geçerli görevin önüne ekleneceği bir görevin. |

### Ayrıca bakınız

* class [Task](../)
* ad alanı [Aspose.Tasks](../../task/)
* toplantı [Aspose.Tasks](../../../)


