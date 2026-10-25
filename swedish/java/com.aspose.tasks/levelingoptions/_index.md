---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange parametrar för resurshantering."
type: docs
weight: 142
url: /sv/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Tillåter att ange parametrar för resurshantering.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Initierar en ny instans av klassen [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Hämtar en token som kan användas för att avbryta en projektutjämningsoperation. |
| [getFinishDate()](#getFinishDate--) | Hämtar slutdatum för utjämningsperioden. |
| [getLevelingOrder()](#getLevelingOrder--) | Hämtar den ordning i vilken utjämningsalgoritmen fördröjer uppgifter som har överallokeringar. |
| [getMessageHandler()](#getMessageHandler--) | Hämtar meddelandehanterarens återuppringning som kan användas för att avlyssna loggmeddelanden som produceras av Aspose.Tasks under resursutjämning. |
| [getMessageLevel()](#getMessageLevel--) | Hämtar nivå på loggmeddelanden som emitteras av Aspose.Tasks under resursutjämning. |
| [getResources()](#getResources--) | Hämtar listan över resurserna som kommer att jämnas. |
| [getStartDate()](#getStartDate--) | Hämtar startdatum för utjämningsperioden. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Ställer in en token som kan användas för att avbryta en projektutjämningsoperation. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Ställer in slutdatum för utjämningsperioden. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | Den ordning i vilken utjämningsalgoritmen fördröjer uppgifter som har överallokeringar. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Ställer in meddelandehanterarens återuppringning som kan användas för att avlyssna loggmeddelanden som produceras av Aspose.Tasks under resursutjämning. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Ställer in nivå på loggmeddelanden som emitteras av Aspose.Tasks under resursutjämning. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Ställer in listan över resurserna som kommer att jämnas. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ställer in startdatum för utjämningsperioden. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Initierar en ny instans av klassen [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Hämtar en token som kan användas för att avbryta en projektutjämningsoperation.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Hämtar slutdatum för utjämningsperioden. Standardvärdet är projektets slutdatum.

**Returns:**
java.util.Date - slutdatum för utjämningsperioden.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Hämtar den ordning i vilken utjämningsalgoritmen fördröjer uppgifter som har överallokeringar. Efter att ha fastställt vilka uppgifter som orsakar överallokeringen och vilka som kan fördröjas, används den angivna ordningen för att bestämma vilken uppgift som ska fördröjas först.

**Returns:**
int - den ordning i vilken utjämningsalgoritmen fördröjer uppgifter som har överallokeringar.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Hämtar meddelandehanterarens återuppringning som kan användas för att avlyssna loggmeddelanden som produceras av Aspose.Tasks under resursutjämning.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Hämtar nivå på loggmeddelanden som emitteras av Aspose.Tasks under resursutjämning.

**Returns:**
int - nivå på loggmeddelanden som emitteras av Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Hämtar listan över resurserna som kommer att jämnas. Om null anges, kommer alla projektresurser att jämnas.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - listan över resurserna som kommer att jämnas.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Hämtar startdatum för utjämningsperioden. Standardvärdet är projektets startdatum.

**Returns:**
java.util.Date - startdatum för nivåinställningsperioden.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Ställer in en token som kan användas för att avbryta en projektutjämningsoperation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | en token som kan användas för att avbryta en projektnivåinställningsoperation. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Ställer in slutdatum för nivåinställningsperioden. Standardvärdet är projektets slutdatum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | slutdatum för nivåinställningsperioden. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


Den ordning i vilken nivåinställningsalgoritmen fördröjer uppgifter som har överallokeringar. Efter att ha identifierat uppgifterna som orsakar överallokeringen och vilka uppgifter som kan fördröjas, används den angivna ordningen för att bestämma vilken uppgift som ska fördröjas först.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ordningen i vilken nivåinställningsalgoritmen fördröjer uppgifter som har överallokeringar. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Ställer in meddelandehanterarens återuppringning som kan användas för att avlyssna loggmeddelanden som produceras av Aspose.Tasks under resursutjämning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | meddelandehanterarens återuppringning som kan användas för att avlyssna loggmeddelanden som produceras av Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Ställer in nivå på loggmeddelanden som emitteras av Aspose.Tasks under resursutjämning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | nivå på loggmeddelanden som emitteras av Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Ställer in listan över resurser som ska nivåinställas. Om null anges, kommer alla projektresurser att nivåinställas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;com.aspose.tasks.Resource&gt; | listan över resurser som ska nivåinställas. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ställer in startdatum för nivåinställningsperioden. Standardvärdet är projektets startdatum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | startdatum för nivåinställningsperioden. |

