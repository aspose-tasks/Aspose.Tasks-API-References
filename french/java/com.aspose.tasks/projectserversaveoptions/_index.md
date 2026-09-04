---
title: "ProjectServerSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lorsque le projet est enregistré sur Project Server ou Project Online."
type: docs
weight: 227
url: /fr/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Permet de spécifier des options supplémentaires lorsque le projet est enregistré sur Project Server ou Project Online.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Initialise une nouvelle instance de la classe [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Obtient l'intervalle entre les requêtes d'état des travaux en file d'attente. |
| [getProjectGuid()](#getProjectGuid--) | Obtient l'identifiant unique d'un projet. |
| [getProjectName()](#getProjectName--) | Obtient le nom d'un projet qui est affiché dans la liste des projets Project Server \\ Project Online. |
| [getTimeout()](#getTimeout--) | Obtient le délai d'attente utilisé lors de l'attente du traitement de la requête de sauvegarde de projet par le service de traitement de file d'attente d'un Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Définit l'intervalle entre les requêtes d'état des travaux en file d'attente. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Définit l'identifiant unique d'un projet. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Définit le nom d'un projet qui est affiché dans la liste des projets Project Server \\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | Définit le délai d'attente utilisé lors de l'attente du traitement de la requête de sauvegarde de projet par le service de traitement de file d'attente d'un Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Initialise une nouvelle instance de la classe [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Obtient l'intervalle entre les requêtes d'état des travaux en file d'attente. La valeur par défaut est de 2 secondes.

**Returns:**
double - intervalle entre les requêtes d'état des travaux en file d'attente.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Obtient l'identifiant unique d'un projet. Doit être unique au sein de l'instance Project Server \\ Project Online.

**Returns:**
java.util.UUID - identifiant unique d'un projet.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Obtient le nom d'un projet qui est affiché dans la liste des projets Project Server \\ Project Online. Doit être unique au sein de l'instance Project Server \\ Project Online. Si la valeur est omise, la valeur de la propriété Prj.Name sera utilisée à la place.

**Returns:**
java.lang.String - nom d'un projet qui est affiché dans la liste des projets Project Server \\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Obtient le délai d'attente utilisé lors de l'attente du traitement de la requête de sauvegarde de projet par le service de traitement de file d'attente d'un Project Server. La valeur par défaut de cette propriété est de 1 minute.

--------------------

Le temps de traitement peut être plus long pour les grands projets ou dans le cas où l'instance de Project Server est trop occupée à répondre à d'autres requêtes.

**Returns:**
double - délai d'attente utilisé lors de l'attente du traitement de la requête d'enregistrement du projet par le service de traitement de la file d'attente de Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Définit l'intervalle entre les demandes d'état des travaux de la file d'attente. La valeur par défaut est de 2 secondes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | intervalle entre les demandes d'état des travaux de la file d'attente. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Définit l'identifiant unique d'un projet. Il doit être unique au sein de l'instance de Project Server \ Project Online.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID | identifiant unique d'un projet. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Définit le nom d'un projet qui est affiché dans la liste des projets de Project Server \ Project Online. Il doit être unique au sein de l'instance de Project Server \ Project Online. Si la valeur est omise, la valeur de la propriété Prj.Name sera utilisée à la place.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | nom d'un projet qui est affiché dans la liste des projets de Project Server \ Project Online. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Définit le délai d'attente utilisé lors de l'attente du traitement de la requête d'enregistrement du projet par le service de traitement de la file d'attente de Project Server. La valeur par défaut pour cette propriété est d'une minute.

--------------------

Le temps de traitement peut être plus long pour les grands projets ou dans le cas où l'instance de Project Server est trop occupée à répondre à d'autres requêtes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | délai d'attente utilisé lors de l'attente du traitement de la requête d'enregistrement du projet par le service de traitement de la file d'attente de Project Server. |

