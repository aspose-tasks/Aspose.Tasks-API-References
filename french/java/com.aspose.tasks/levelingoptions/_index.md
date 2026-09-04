---
title: "LevelingOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier les paramètres de nivellement des ressources."
type: docs
weight: 142
url: /fr/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Permet de spécifier les paramètres de nivellement des ressources.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Initialise une nouvelle instance de la classe [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Obtient un jeton qui peut être utilisé pour annuler une opération de nivellement de projet. |
| [getFinishDate()](#getFinishDate--) | Obtient la date de fin de la période de nivellement. |
| [getLevelingOrder()](#getLevelingOrder--) | Obtient l'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations. |
| [getMessageHandler()](#getMessageHandler--) | Obtient le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par Aspose.Tasks lors du nivellement des ressources. |
| [getMessageLevel()](#getMessageLevel--) | Obtient le niveau des messages de journal émis par Aspose.Tasks lors du nivellement des ressources. |
| [getResources()](#getResources--) | Obtient la liste des ressources qui seront nivelées. |
| [getStartDate()](#getStartDate--) | Obtient la date de début de la période de nivellement. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Définit un jeton qui peut être utilisé pour annuler une opération de nivellement de projet. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Définit la date de fin de la période de nivellement. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | L'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Définit le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par **Aspose.Tasks** lors du nivellement des ressources. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Définit le niveau des messages de journal émis par **Aspose.Tasks** lors du nivellement des ressources. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Définit la liste des ressources qui seront nivelées. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Définit la date de début de la période de nivellement. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Initialise une nouvelle instance de la classe [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Obtient un jeton qui peut être utilisé pour annuler une opération de nivellement de projet.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Obtient la date de fin de la période de nivellement. La valeur par défaut est la date de fin du projet`s.

**Returns:**
java.util.Date - date de fin de la période de nivellement.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Obtient l'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations. Après la détermination des tâches causant la surallocation et des tâches pouvant être retardées, l'ordre spécifié est utilisé pour déterminer quelle tâche doit être retardée en premier.

**Returns:**
int - l'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Obtient le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par Aspose.Tasks lors du nivellement des ressources.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Obtient le niveau des messages de journal émis par Aspose.Tasks lors du nivellement des ressources.

**Returns:**
int - niveau des messages de journal émis par **Aspose**.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Obtient la liste des ressources qui seront nivelées. Si null est défini, toutes les ressources du projet seront nivelées.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - la liste des ressources qui seront nivelées.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtient la date de début de la période de nivellement. La valeur par défaut est la date de début du projet`s.

**Returns:**
java.util.Date - date de début de la période de nivellement.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Définit un jeton qui peut être utilisé pour annuler une opération de nivellement de projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un jeton qui peut être utilisé pour annuler une opération de nivellement de projet. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Définit la date de fin de la période de nivellement. La valeur par défaut est la date de fin du projet`s.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | date de fin de la période de nivellement. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


L'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations. Après la détermination des tâches causant la surallocation et des tâches pouvant être retardées, l'ordre spécifié est utilisé pour déterminer quelle tâche doit être retardée en premier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'ordre dans lequel l'algorithme de nivellement retarde les tâches qui ont des surallocations. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Définit le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par **Aspose.Tasks** lors du nivellement des ressources.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par **Aspose**. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Définit le niveau des messages de journal émis par **Aspose.Tasks** lors du nivellement des ressources.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | niveau des messages de journal émis par **Aspose**. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Définit la liste des ressources qui seront nivelées. Si null est défini, toutes les ressources du projet seront nivelées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;com.aspose.tasks.Resource&gt; | la liste des ressources qui seront nivelées. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Définit la date de début de la période de nivellement. La valeur par défaut est la date de début du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | date de début de la période de nivellement. |

