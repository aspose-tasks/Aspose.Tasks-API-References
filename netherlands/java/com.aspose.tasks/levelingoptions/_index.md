---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe parameters van resource-leveling op te geven."
type: docs
weight: 142
url: /nl/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Staat toe parameters van resource-leveling op te geven.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Initialiseert een nieuw exemplaar van de klasse [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Haalt een token op dat kan worden gebruikt om een project-levelingbewerking te annuleren. |
| [getFinishDate()](#getFinishDate--) | Haalt de einddatum van de levelingperiode op. |
| [getLevelingOrder()](#getLevelingOrder--) | Haalt de volgorde op waarin het leveling-algoritme taken met overallocaties vertraagt. |
| [getMessageHandler()](#getMessageHandler--) | Haalt de callback van de berichtafhandelaar op die kan worden gebruikt om logberichten, geproduceerd door Aspose.Tasks tijdens resource-leveling, te onderscheppen. |
| [getMessageLevel()](#getMessageLevel--) | Haalt het niveau van logberichten op die door Aspose.Tasks tijdens resource-leveling worden uitgezonden. |
| [getResources()](#getResources--) | Haalt de lijst op van de resources die genivelleerd zullen worden. |
| [getStartDate()](#getStartDate--) | Haalt de begindatum van de nivelleringstermijn op. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Stelt een token in dat kan worden gebruikt om een projectniveleeroperatie te annuleren. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Stelt de einddatum van de nivelleringstermijn in. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | De volgorde waarin het nivelleringalgoritme taken met overallocaties vertraagt. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Stelt een callback voor berichtafhandeling in die kan worden gebruikt om logberichten die door Aspose.Tasks tijdens resource-nivellering worden geproduceerd, af te vangen. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Stelt het niveau van logberichten in die door Aspose.Tasks tijdens resource-nivellering worden uitgegeven. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Stelt de lijst in van de resources die genivelleerd zullen worden. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Stelt de begindatum van de nivelleringstermijn in. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Initialiseert een nieuw exemplaar van de klasse [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Haalt een token op dat kan worden gebruikt om een project-levelingbewerking te annuleren.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Haalt de einddatum van de nivelleringstermijn op. De standaardwaarde is de einddatum van het project`s.

**Returns:**
java.util.Date - einddatum van de nivelleringstermijn.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Haalt de volgorde op waarin het nivelleringalgoritme taken met overallocaties vertraagt. Na het bepalen van de taken die de overallocatie veroorzaken en welke taken kunnen worden vertraagd, wordt de opgegeven volgorde gebruikt om te bepalen welke taak eerst moet worden vertraagd.

**Returns:**
int - de volgorde waarin het nivelleringalgoritme taken met overallocaties vertraagt.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Haalt de callback van de berichtafhandelaar op die kan worden gebruikt om logberichten, geproduceerd door Aspose.Tasks tijdens resource-leveling, te onderscheppen.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Haalt het niveau van logberichten op die door Aspose.Tasks tijdens resource-leveling worden uitgezonden.

**Returns:**
int - niveau van logberichten uitgegeven door Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Haalt de lijst op van de resources die genivelleerd zullen worden. Als null is ingesteld, worden alle projectresources genivelleerd.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - de lijst van de resources die genivelleerd zullen worden.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Haalt de begindatum van de nivelleringstermijn op. De standaardwaarde is de startdatum van het project`s.

**Returns:**
java.util.Date - begindatum van de nivelleringstermijn.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Stelt een token in dat kan worden gebruikt om een projectniveleeroperatie te annuleren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | een token die kan worden gebruikt om een projectniveleeroperatie te annuleren. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Stelt de einddatum van de nivelleringstermijn in. De standaardwaarde is de einddatum van het project`s.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | einddatum van de nivelleringstermijn. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


De volgorde waarin het nivelleringalgoritme taken met overallocaties vertraagt. Na het bepalen van de taken die de overallocatie veroorzaken en welke taken kunnen worden vertraagd, wordt de opgegeven volgorde gebruikt om te bepalen welke taak eerst moet worden vertraagd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de volgorde waarin het nivelleringalgoritme taken met overallocaties vertraagt. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Stelt een callback voor berichtafhandeling in die kan worden gebruikt om logberichten die door Aspose.Tasks tijdens resource-nivellering worden geproduceerd, af te vangen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | berichtafhandelingscallback die kan worden gebruikt om logberichten die door Aspose worden geproduceerd, af te vangen. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Stelt het niveau van logberichten in die door Aspose.Tasks tijdens resource-nivellering worden uitgegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | niveau van logberichten uitgegeven door Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Stelt de lijst van de resources in die genivelleerd zullen worden. Als null is ingesteld, worden alle projectresources genivelleerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.List&lt;com.aspose.tasks.Resource&gt; | de lijst van de resources die genivelleerd zullen worden. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Stelt de startdatum van de nivelleringperiode in. De standaardwaarde is de startdatum van het project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | startdatum van de nivelleringperiode. |

