---
title: Task
second_title: Aspose.Tasks for .NET API Referansı
description: Bir projedeki görevi temsil eder.
type: docs
weight: 2060
url: /tr/net/aspose.tasks/task/
---
## Task class

Bir projedeki görevi temsil eder.

```csharp
public class Task : IEquatable<Task>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Bu nesne için kaynak atamalarının bir koleksiyonunu alır. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Görevin temel değerlerinin koleksiyonunu alır veya ayarlar. |
| [Children](../../aspose.tasks/task/children) { get; } | Bu nesnenin bir alt görev koleksiyonunu alır. Alt görevleri temsil eden TaskCollection nesnesi. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Genişletilmiş bir özniteliğin değerlerini içeren ExtendedAttributeCollection nesnesini alır. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Alır veya ayarlar[`OutlineCodeCollection`](../outlinecodecollection) nesne. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Bir görevin üst projesini alır. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Bir görevin üst görevini alır. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | [`TaskCollection`](../taskcollection) bu Task nesnesinin tüm öncüllerini içeren nesne. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Örneğini alır[`RecurringTaskInfo`](../recurringtaskinfo) yinelenen bir görev olan görev için sınıf; görev yinelenen bir görev değilse null; döndürür örneği için bilgi[`RecurringTaskInfo`](../recurringtaskinfo) yalnızca mpp dosya biçiminde bulunur. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Bir görevin bölümlerini temsil eden bir SplitPart koleksiyonu alır. |
| [Successors](../../aspose.tasks/task/successors) { get; } | [`TaskCollection`](../taskcollection) bu Task nesnesinin tüm ardıllarını içeren nesne. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Bu görevin TimephasedDataCollection nesnesini alır veya ayarlar. Bir görevle ilişkili zaman aşamalı veri bloğu. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Alt görevler olmadan görevin tam kopyasını oluşturur. |
| [Delete](../../aspose.tasks/task/delete)() | Üst proje görevleri koleksiyonundan ve tüm atamalarından bir görevi siler. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Bu örneğin belirtilen bir göreve eşit olup olmadığını gösteren bir değer döndürür. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Özelliğin bu kapsayıcıda eşlendiği değeri döndürür. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Bu Görev için bir karma kod değeri döndürür. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | İade[`TimephasedDataCollection`](../timephaseddatacollection) ile nesne[`TimephasedData`](./timephaseddata) verilen başlangıç ve bitiş tarihlerindeki değerler. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | İade[`TimephasedDataCollection`](../timephaseddatacollection) ile nesne[`TimephasedData`](./timephaseddata) belirtilen zaman aşamalı veri türünün verilen başlangıç ve bitiş tarihleri içindeki değerler. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Geçerli görevi belirtilen Kimliğe sahip bir görevden önce aynı Anahat Düzeyinde taşır. ParentProject.CalculationMode Yok ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate() öğesini çağırmalıdır (Tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) ve bolluklar, iş ve maliyet alanları, anahat seviyeleri gibi bağımlı alanları hesaplayın). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, anahat seviyesini ve anahat numaralarını otomatik olarak hesaplayacaktır. ParentProject ise. CalculationMode Otomatiktir Yöntem, tüm projenin görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, bollukları, iş ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Geçerli görevi belirtilen görevden önce aynı Anahat Düzeyinde taşır. ParentProject.CalculationMode Hiçbiri ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate() öğesini çağırmalıdır (Tüm proje görevlerini yeniden planlar (başlangıç/bitiş tarihleri, erken ayarlar/ geç tarihler) ve bolluklar, iş ve maliyet alanları, anahat seviyeleri gibi bağımlı alanları hesaplayın). ParentProject.CalculationMode Manuel ise, yöntem yalnızca görev kimliğini, anahat seviyesini ve anahat numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Otomatik ise yöntem tüm proje görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, bollukları, iş ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Anahatta bir görevi girintiler. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Anahatta bir görevi ilerletir. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Bu görevin tüm alt görevlerini yinelemeli olarak toplar. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Belirtilen özelliği bu kapsayıcıda belirtilen değerle eşler. |
| override [ToString](../../aspose.tasks/task/tostring)() | Bir görevin kısa dize gösterimini döndürür. Gösterimin tam ayrıntıları belirtilmemiştir ve değiştirilebilir. |

### Notlar

bu **Görev** tek atomik bir iş parçasını temsil ediyor.

Kullanılabilir **Görev**görevler oluşturarak bir proje planlamak ve bunlara uygun kaynakları atamak. Bir projedeki görevler, bir kök görev ve alt görevlerin alt ağaçları ile köklü bir hiyerarşik ağaç yapısı olarak düzenlenir.

Bir görev ağacı oluşturmak için özel bir koleksiyon kullanılabilir.[`TaskCollection`](../taskcollection) erişerek[`RootTask`](../project/roottask) mülk örneğin:

```csharp
Project project = new Project();

// yeni görevler ekle
Task task1 = project.RootTask.Children.Add(); // adı boş olan bir üst görev eklendi
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // childTask3'ten önce bir görev ekler
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// projeyi mevcut formatlardan birinde kaydedin
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
