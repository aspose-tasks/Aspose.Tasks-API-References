---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven wanneer het project wordt opgeslagen op Project Server of Project Online."
type: docs
weight: 227
url: /nl/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Staat toe extra opties op te geven wanneer het project wordt opgeslagen op Project Server of Project Online.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Initialiseert een nieuw exemplaar van de [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Haalt het interval op tussen verzoeken voor de status van wachtrijtaken. |
| [getProjectGuid()](#getProjectGuid--) | Haalt de unieke identifier van een project op. |
| [getProjectName()](#getProjectName--) | Haalt de naam op van een project die wordt weergegeven in de Project Server \\ Project Online projectenlijst. |
| [getTimeout()](#getTimeout--) | Haalt de time-out op die wordt gebruikt bij het wachten op de verwerking van een opslaan-projectverzoek door de wachtrijverwerkingsservice van Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Stelt het interval in tussen verzoeken voor de status van wachtrijtaken. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Stelt de unieke identifier van een project in. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Stelt de naam in van een project die wordt weergegeven in de Project Server \\ Project Online projectenlijst. |
| [setTimeout(double value)](#setTimeout-double-) | Stelt de time-out in die wordt gebruikt bij het wachten op de verwerking van een opslaan-projectverzoek door de wachtrijverwerkingsservice van Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Initialiseert een nieuw exemplaar van de [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) klasse.

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Haalt het interval op tussen verzoeken voor de status van wachtrijtaken. De standaardwaarde is 2 seconden.

**Returns:**
double - interval tussen verzoeken voor de status van wachtrijtaken.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Haalt de unieke identifier van een project op. Moet uniek zijn binnen de Project Server \\ Project Online instantie.

**Returns:**
java.util.UUID - unieke identifier van een project.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Haalt de naam op van een project die wordt weergegeven in de Project Server \\ Project Online projectenlijst. Moet uniek zijn binnen de Project Server \\ Project Online instantie. Als de waarde wordt weggelaten, wordt de waarde van de Prj.Name‑eigenschap gebruikt.

**Returns:**
java.lang.String - naam van een project die wordt weergegeven in de Project Server \\ Project Online projectenlijst.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Haalt de time-out op die wordt gebruikt bij het wachten op de verwerking van een opslaan-projectverzoek door de wachtrijverwerkingsservice van Project Server. De standaardwaarde voor deze eigenschap is 1 minuut.

--------------------

De verwerkingstijd kan langer zijn voor grote projecten of in het geval dat de Project Server‑instantie te druk is met het beantwoorden van andere verzoeken.

**Returns:**
double - time‑out gebruikt bij het wachten op de verwerking van een opslaan‑project‑verzoek door de wachtrij‑verwerkingsservice van een Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Stelt het interval tussen wachtrij‑taakstatusaanvragen in. De standaardwaarde is 2 seconden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | interval tussen wachtrij‑taakstatusaanvragen. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Stelt de unieke identifier van een project in. Moet uniek zijn binnen de Project Server \ Project Online‑instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.UUID | unieke identifier van een project. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Stelt de naam van een project in die wordt weergegeven in de Project Server \ Project Online‑projectenlijst. Moet uniek zijn binnen de Project Server \ Project Online‑instantie. Als de waarde wordt weggelaten, wordt de waarde van de Prj.Name‑eigenschap gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | naam van een project die wordt weergegeven in de Project Server \ Project Online‑projectenlijst. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Stelt de time‑out in die wordt gebruikt bij het wachten op de verwerking van een opslaan‑project‑verzoek door de wachtrij‑verwerkingsservice van een Project Server. De standaardwaarde voor deze eigenschap is 1 minuut.

--------------------

De verwerkingstijd kan langer zijn voor grote projecten of in het geval dat de Project Server‑instantie te druk is met het beantwoorden van andere verzoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | time‑out gebruikt bij het wachten op de verwerking van een opslaan‑project‑verzoek door de wachtrij‑verwerkingsservice van een Project Server. |

