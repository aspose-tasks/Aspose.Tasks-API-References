---
title: "MPPSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors de l'enregistrement des données du projet au format MPP."
type: docs
weight: 149
url: /fr/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors de l'enregistrement des données du projet au format MPP.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Initialise une nouvelle instance de la classe [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getClearVba()](#getClearVba--) | Obtient une valeur indiquant s'il faut supprimer les données de macros VBA existantes lors de l'enregistrement d'un projet au format MPP. |
| [getProtectionPassword()](#getProtectionPassword--) | Obtient un mot de passe utilisé pour protéger le fichier MPP résultant. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Obtient une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. |
| [getWriteFilters()](#getWriteFilters--) | Obtient une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. |
| [getWriteGroups()](#getWriteGroups--) | Obtient une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. |
| [getWriteVba()](#getWriteVba--) | Obtient une valeur indiquant s'il faut mettre à jour les données des macros VBA existantes dans le fichier MPP. |
| [getWriteViewData()](#getWriteViewData--) | Obtient une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Définit une valeur indiquant s'il faut supprimer les données des macros VBA existantes lors de l'enregistrement d'un projet au format MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Définit un mot de passe utilisé pour protéger le fichier MPP résultant. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Définit une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Définit une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Définit une valeur indiquant s'il faut mettre à jour les données des macros VBA existantes dans le fichier MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Définit une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initialise une nouvelle instance de la classe [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Obtient une valeur indiquant s'il faut supprimer les données de macros VBA existantes lors de l'enregistrement d'un projet au format MPP.

**Returns:**
booléen - une valeur indiquant s'il faut supprimer les données des macros VBA existantes lors de l'enregistrement d'un projet au format MPP.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Obtient un mot de passe utilisé pour protéger le fichier MPP résultant. Actuellement pris en charge pour les formats MS Project 2010 et ultérieurs.

--------------------

Une valeur nulle indique que le fichier de projet n'est pas protégé.

**Returns:**
java.lang.String - un mot de passe utilisé pour protéger le fichier MPP résultant.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Obtient une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP.

--------------------

MS Project crée une affectation de ressource vide pour chaque tâche. Définissez ce drapeau sur true pour les supprimer lors de l'enregistrement.

**Returns:**
booléen - une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Obtient une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de filtre incluent les collections Project.TaskFilters et Project.ResourceFilters.

--------------------

Actuellement pris en charge pour les formats MSP 2010 ou ultérieurs.

**Returns:**
booléen - une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Obtient une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de groupe incluent les collections Project.TaskGroups et Project.ResourceGroups.

**Returns:**
booléen - une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Obtient une valeur indiquant s'il faut mettre à jour les données des macros VBA existantes dans le fichier MPP. L'écriture de VbaModule.SourceCode est actuellement prise en charge.

**Returns:**
booléen - une valeur indiquant s'il faut mettre à jour les données des macros VBA existantes dans le fichier MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Obtient une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de vue incluent les collections Project.Views, Filters et Tables.

**Returns:**
booléen - une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Définit une valeur indiquant s'il faut supprimer les données des macros VBA existantes lors de l'enregistrement d'un projet au format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut supprimer les données de macros VBA existantes lors de l'enregistrement d'un projet au format MPP. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Définit un mot de passe utilisé pour protéger le fichier MPP résultant. Actuellement pris en charge pour les formats MS Project 2010 et ultérieurs.

--------------------

Une valeur nulle indique que le fichier de projet n'est pas protégé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un mot de passe utilisé pour protéger le fichier MPP résultant. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP.

--------------------

MS Project crée une affectation de ressource vide pour chaque tâche. Définissez ce drapeau sur true pour les supprimer lors de l'enregistrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Définit une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de filtre incluent les collections Project.TaskFilters et Project.ResourceFilters.

--------------------

Actuellement pris en charge pour les formats MSP 2010 ou ultérieurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Définit une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de groupe incluent les collections Project.TaskGroups et Project.ResourceGroups.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Définit une valeur indiquant s'il faut mettre à jour les données de macros VBA existantes dans le fichier MPP. L'écriture de VbaModule.SourceCode est actuellement prise en charge.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut mettre à jour les données de macros VBA existantes dans le fichier MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Définit une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP.

--------------------

Les données de vue incluent les collections Project.Views, Filters et Tables.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. |

