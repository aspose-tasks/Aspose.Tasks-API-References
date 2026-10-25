---
title: "PrimaveraXmlSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera xml."
type: docs
weight: 212
url: /fr/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera xml.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Initialise une nouvelle instance de la classe [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Obtient une valeur indiquant s'il faut enregistrer une tâche racine ou non. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Obtient une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Définit une valeur indiquant s'il faut enregistrer une tâche racine ou non. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Initialise une nouvelle instance de la classe [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Obtient une valeur indiquant s'il faut enregistrer une tâche racine ou non.

**Returns:**
booléen - une valeur indiquant s'il faut enregistrer une tâche racine ou non.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Obtient une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation.

Le logiciel Primavera ne prend pas en charge l'affectation de ressources aux tâches de synthèse (WBS). Ainsi, l'exportation de ces affectations peut entraîner un fichier invalide selon le modèle de Primavera. Si vrai, les affectations aux tâches de synthèse sont ignorées lors de l'exportation. Si faux (valeur par défaut), une exception sera levée si une affectation à une tâche de synthèse est rencontrée lors de l'exportation.

**Returns:**
booléen - une valeur indiquant si les affectations de ressources aux tâches de synthèse doivent être ignorées lors de l'exportation.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Définit une valeur indiquant s'il faut enregistrer une tâche racine ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut enregistrer une tâche racine ou non. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation.

Le logiciel Primavera ne prend pas en charge l'affectation de ressources aux tâches de synthèse (WBS). Ainsi, l'exportation de ces affectations peut entraîner un fichier invalide selon le modèle de Primavera. Si vrai, les affectations aux tâches de synthèse sont ignorées lors de l'exportation. Si faux (valeur par défaut), une exception sera levée si une affectation à une tâche de synthèse est rencontrée lors de l'exportation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les affectations de ressources aux tâches de synthèse doivent être ignorées lors de l'exportation. |

