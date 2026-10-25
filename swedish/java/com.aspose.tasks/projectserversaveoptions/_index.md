---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektet sparas till Project Server eller Project Online."
type: docs
weight: 227
url: /sv/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Tillåter att ange ytterligare alternativ när projektet sparas till Project Server eller Project Online.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Initierar en ny instans av klassen [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Hämtar intervallet mellan förfrågningar om köjobbsstatus. |
| [getProjectGuid()](#getProjectGuid--) | Hämtar unik identifierare för ett projekt. |
| [getProjectName()](#getProjectName--) | Hämtar namn på ett projekt som visas i Project Server \\ Project Online-projektlista. |
| [getTimeout()](#getTimeout--) | Hämtar timeout som används när man väntar på bearbetning av spara-projekt-förfrågan av Project Servers köbearbetningstjänst. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Ställer in intervallet mellan förfrågningar om köjobbsstatus. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Ställer in unik identifierare för ett projekt. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Ställer in namn på ett projekt som visas i Project Server \\ Project Online-projektlista. |
| [setTimeout(double value)](#setTimeout-double-) | Ställer in timeout som används när man väntar på bearbetning av spara projekt‑begäran av en Project Server:s köbearbetningstjänst. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Initierar en ny instans av klassen [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Hämtar intervallet mellan köjobbsstatusförfrågningar. Standardvärdet är 2 sekunder.

**Returns:**
double - intervall mellan köjobbsstatusförfrågningar.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Hämtar unik identifierare för ett projekt. Ska vara unik inom en Project Server \\ Project Online-instans.

**Returns:**
java.util.UUID - unik identifierare för ett projekt.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Hämtar namn på ett projekt som visas i Project Server \\ Project Online-projektslistan. Ska vara unik inom en Project Server \\ Project Online-instans. Om värdet utelämnas används värdet från egenskapen Prj.Name istället.

**Returns:**
java.lang.String - namn på ett projekt som visas i Project Server \\ Project Online-projektslistan.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Hämtar timeout som används när man väntar på bearbetning av spara projekt‑begäran av en Project Server:s köbearbetningstjänst. Standardvärdet för denna egenskap är 1 minut.

--------------------

Bearbetningstiden kan vara längre för stora projekt eller om Project Server‑instansen är för upptagen med att svara på andra förfrågningar.

**Returns:**
double - timeout som används när man väntar på bearbetning av spara projekt‑begäran av en Project Server:s köbearbetningstjänst.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Ställer in intervallet mellan köjobbsstatusförfrågningar. Standardvärdet är 2 sekunder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | intervall mellan köjobbsstatusförfrågningar. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Ställer in unik identifierare för ett projekt. Ska vara unik inom en Project Server \\ Project Online-instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID | unik identifierare för ett projekt. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Ställer in namn på ett projekt som visas i Project Server \\ Project Online-projektslistan. Ska vara unik inom en Project Server \\ Project Online-instans. Om värdet utelämnas används värdet från egenskapen Prj.Name istället.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namn på ett projekt som visas i Project Server \\ Project Online-projektslistan. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Ställer in timeout som används när man väntar på bearbetning av spara projekt‑begäran av en Project Server:s köbearbetningstjänst. Standardvärdet för denna egenskap är 1 minut.

--------------------

Bearbetningstiden kan vara längre för stora projekt eller om Project Server‑instansen är för upptagen med att svara på andra förfrågningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | timeout som används när man väntar på bearbetning av spara projekt‑begäran av en Project Server:s köbearbetningstjänst. |

