---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Kaynak dengeleme yöntemlerini içerir."
type: docs
weight: 253
url: /tr/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Kaynak dengeleme yöntemlerini içerir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Kaynak dengelemesi sırasında projeye daha önce eklenmiş olan herhangi bir dengeleme gecikmesini temizler. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Kaynak dengelemesi sırasında belirtilen görevlere daha önce eklenen tüm dengeleme gecikmelerini temizler. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Projenin tüm kaynakları için görevleri varsayılan dengeleme seçeneklerini kullanarak dengeler. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Belirtilen kaynaklar için görevleri belirtilen dengeleme seçeneklerini kullanarak dengeler. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Kaynak dengelemesi sırasında projeye daha önce eklenmiş olan herhangi bir dengeleme gecikmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Dengelemeyi temizlemek için proje. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Kaynak dengelemesi sırasında belirtilen görevlere daha önce eklenen tüm dengeleme gecikmelerini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görevler | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | Dengeleme gecikmesinin temizlenmesi gereken görevleri içeren enumerable. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Projenin tüm kaynakları için görevleri varsayılan dengeleme seçeneklerini kullanarak dengeler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Kaynak dengelemesini uygulamak için proje. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Belirtilen kaynaklar için görevleri belirtilen dengeleme seçeneklerini kullanarak dengeler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Kaynak dengelemesini uygulamak için proje. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Kaynakların nasıl dengeleceğini belirten seçenekler. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
