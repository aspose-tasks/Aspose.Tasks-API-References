---
title: "ResourceLeveler"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Contient des méthodes d'équilibrage des ressources."
type: docs
weight: 253
url: /fr/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Contient des méthodes d'équilibrage des ressources.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Supprime tout délai d'équilibrage qui a été précédemment ajouté au projet lors de l'équilibrage des ressources. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Supprime tout délai d'équilibrage qui avait été précédemment ajouté aux tâches spécifiées pendant l'équilibrage des ressources. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Équilibre les tâches pour toutes les ressources du projet en utilisant les options d'équilibrage par défaut. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Équilibre les tâches pour les ressources spécifiées en utilisant les options d'équilibrage spécifiées. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Supprime tout délai d'équilibrage qui a été précédemment ajouté au projet lors de l'équilibrage des ressources.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projet pour supprimer l'équilibrage. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Supprime tout délai d'équilibrage qui avait été précédemment ajouté aux tâches spécifiées pendant l'équilibrage des ressources.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tâches | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | L'énumérable contenant les tâches pour lesquelles le délai d'équilibrage doit être supprimé. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Équilibre les tâches pour toutes les ressources du projet en utilisant les options d'équilibrage par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projet pour appliquer l'équilibrage des ressources. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Équilibre les tâches pour les ressources spécifiées en utilisant les options d'équilibrage spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projet pour appliquer l'équilibrage des ressources. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Options qui spécifient comment équilibrer les ressources. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
