---
title: "PrimaveraReadOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors de la lecture de fichiers Primavera Xml ou Primavera Xer."
type: docs
weight: 206
url: /fr/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Permet de spécifier des options supplémentaires lors de la lecture de fichiers Primavera Xml ou Primavera Xer.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Initialise une nouvelle instance de la classe [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Obtient un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés. |
| [getProjectUid()](#getProjectUid--) | Obtient l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Obtient un indicateur qui spécifie si les projets de référence doivent être chargés. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Spécifie le comportement utilisé pour traiter les tâches avec des contraintes non définies lues au format XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Définit un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés. |
| [setProjectUid(int value)](#setProjectUid-int-) | Définit l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Définit un indicateur qui spécifie si les projets de référence doivent être chargés. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Spécifie le comportement utilisé pour traiter les tâches avec des contraintes non définies lues au format XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Initialise une nouvelle instance de la classe [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Obtient un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés.

**Returns:**
booléen - un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Obtient l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets.

**Returns:**
int - l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Obtient un indicateur qui spécifie si les projets de référence doivent être chargés. La valeur par défaut est true.

--------------------

L'indicateur s'applique aux fichiers Primavera XML contenant des projets de référence (les références ne sont pas prises en charge par le format XER). L'option peut être définie sur false pour accélérer le chargement d'un grand projet avec des références lorsque les données de référence ne sont pas nécessaires.

**Returns:**
booléen - un indicateur qui spécifie si les projets de référence doivent être chargés.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Spécifie le comportement utilisé pour traiter les tâches avec des contraintes non définies lues au format XER.

**Returns:**
int - le comportement utilisé pour traiter les tâches avec des contraintes non définies lues au format XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Définit un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | un indicateur qui spécifie si les identifiants uniques d'origine des entités doivent être conservés. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Définit l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Définit un indicateur qui spécifie si les projets de référence doivent être chargés. La valeur par défaut est vraie.

--------------------

L'indicateur s'applique aux fichiers Primavera XML contenant des projets de référence (les références ne sont pas prises en charge par le format XER). L'option peut être définie sur false pour accélérer le chargement d'un grand projet avec des références lorsque les données de référence ne sont pas nécessaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | un indicateur qui spécifie si les projets de référence doivent être chargés. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Spécifie le comportement utilisé pour traiter les tâches avec des contraintes non définies lues au format XER.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le comportement utilisé pour traiter les tâches avec des contraintes indéfinies lues à partir du format XER. |

