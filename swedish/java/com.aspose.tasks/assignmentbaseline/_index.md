---
title: "AssignmentBaseline"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar Baseline för en resursallokering."
type: docs
weight: 17
url: /sv/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

Representerar Baseline för en resursallokering.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | Implementering av IComparable‑gränssnittet. |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getFinish()](#getFinish--) | Hämtar det planerade slutdatumet för resursuppdraget när baslinjen sparades. |
| [getStart()](#getStart--) | Hämtar det planerade startdatumet för resursuppdraget när baslinjen sparades. |
| [getTimephasedData()](#getTimephasedData--) | Hämtar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-instansen för detta objekt. |
| [hashCode()](#hashCode--) | Returnerar ett hash‑kodvärde för detta AssignmentBaseline. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ställer in det planerade slutdatumet för resursuppdraget när baslinjen sparades. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ställer in det planerade startdatumet för resursuppdraget när baslinjen sparades. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ställer in [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-instansen för detta objekt. |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


Implementering av IComparable‑gränssnittet. Jämför denna instans med det angivna Baseline‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | det angivna Baseline‑objektet att jämföra denna instans med. |

**Returns:**
int – returnerar -1 om denna instans är mindre än det angivna objektet, 1 om den är större än det angivna objektet; annars returneras 0.
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | det angivna AssignmentBaseline-objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna AssignmentBaseline-objektet; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | det angivna objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna objektet; annars false.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Hämtar det planerade slutdatumet för resursuppdraget när baslinjen sparades.

Värde: Slutdatumet för resursuppdraget när denna baslinje sparades.

**Returns:**
java.util.Date – det planerade slutdatumet för resursuppdraget när baslinjen sparades.
### getStart() {#getStart--}
```
public final Date getStart()
```


Hämtar det planerade startdatumet för resursuppdraget när baslinjen sparades.

Värde: Startdatumet för resursallokeringen när denna baslinje sparades.

**Returns:**
java.util.Date - det planerade startdatumet för resursallokeringen när baslinjen sparades.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Hämtar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-instansen för detta objekt. Den tidsfasade data som är associerad med resursallokeringsbaslinjen.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hash‑kodvärde för detta AssignmentBaseline.

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ställer in det planerade slutdatumet för resursuppdraget när baslinjen sparades.

Värde: Slutdatumet för resursuppdraget när denna baslinje sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det planerade slutdatumet för resursallokeringen när baslinjen sparades. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ställer in det planerade startdatumet för resursuppdraget när baslinjen sparades.

Värde: Startdatumet för resursallokeringen när denna baslinje sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det planerade startdatumet för resursallokeringen när baslinjen sparades. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ställer in [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-instansen för detta objekt. Den tidsfasade data som är associerad med resursallokeringsbaslinjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | den [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-instansen för detta objekt. |

