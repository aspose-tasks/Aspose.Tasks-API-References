---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett enskilt lager av tidslinjen i ett Gantt-diagram."
type: docs
weight: 325
url: /sv/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Representerar ett enskilt lager av tidslinjen i ett Gantt-diagram.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Initierar en ny instans av klassen [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Initierar en ny instans av klassen [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAlignment()](#getAlignment--) | Hämtar hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Hämtar tidsenhetsintervallet som etiketter ska visas för i nivån. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Hämtar en återuppringningsfunktion för att hantera rendering av datumsteg i den här nivån. |
| [getLabel()](#getLabel--) | Hämtar datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Hämtar flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor. |
| [getShowTicks()](#getShowTicks--) | Hämtar ett värde som anger om tick-markeringar som separerar tidsperioder i nivån ska visas. |
| [getUnit()](#getUnit--) | Hämtar tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Hämtar ett värde som anger om nivåetiketterna ska baseras på räkenskapsåret. |
| [setAlignment(int value)](#setAlignment-int-) | Ställer in hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Ställer in tidsenhetsintervallet som etiketter ska visas för i nivån. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Ställer in en återuppringningsfunktion för att hantera rendering av datumsteg i den här nivån. |
| [setLabel(int value)](#setLabel-int-) | Ställer in datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Ställer in flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Ställer in ett värde som anger om tick-markeringar som separerar tidsperioder i nivån ska visas. |
| [setUnit(int value)](#setUnit-int-) | Ställer in tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Ställer in ett värde som anger om nivåetiketterna ska baseras på räkenskapsåret. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Initierar en ny instans av klassen [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Initierar en ny instans av klassen [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| unit | int | Tidslinjeenheten [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Antalet [TimescaleUnit](../../com.aspose.tasks/timescaleunit)-enheter. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Hämtar hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Hämtar tidsenhetsintervallet som etiketter ska visas för i nivån. Standardvärdet är 1.

**Returns:**
int - tidsenhetsintervallet som etiketter ska visas för i nivån.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Hämtar en återuppringningsfunktion för att hantera rendering av datumsteg i den här nivån.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Hämtar datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån.

**Returns:**
int - datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Hämtar flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor. Om värdet är 'true' renderas datumetiketter för perioden på varje sida när tidsperioden sträcker sig över flera sidor. Om värdet är 'false' renderas datumetiketten endast en gång enligt värdet av `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) egenskapen.

--------------------

Har ingen motsvarighet i MS Project.

**Returns:**
boolean - flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Hämtar ett värde som anger om tick-markeringar som separerar tidsperioder i nivån ska visas.

**Returns:**
boolean - ett värde som indikerar om huruvida tick-markeringar som separerar tidsperioder i nivån ska visas.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Hämtar tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån. Standardvärdet är [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Hämtar ett värde som anger om nivåetiketterna ska baseras på räkenskapsåret.

**Returns:**
boolean - ett värde som indikerar om nivåetiketterna ska baseras på räkenskapsåret.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Ställer in hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | hur etiketter ska justeras inom varje tidsperiod i nivån ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Ställer in tidsenhetsintervallet där etiketter för nivån ska visas. Standardvärdet är 1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | tidsenhetsintervallet där etiketter för nivån ska visas. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Ställer in en återuppringningsfunktion för att hantera rendering av datumsteg i den här nivån.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | en återuppringningsfunktion för att hantera rendering av datum-tick i denna nivå. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Ställer in datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | datumetikett [DateLabel](../../com.aspose.tasks/datelabel) för tidslinjenivån. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Ställer in flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor. Om värdet är 'true' renderas datumetiketter för perioden på varje sida när tidsperioden sträcker sig över flera sidor. Om värdet är 'false' renderas datumetiketten endast en gång enligt värdet av `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) egenskapen.

--------------------

Har ingen motsvarighet i MS Project.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | flagga som definierar om datumetiketter ska renderas på varje sida när en tidsperiod sträcker sig över flera sidor. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Ställer in ett värde som anger om tick-markeringar som separerar tidsperioder i nivån ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om huruvida tick-markeringar som separerar tidsperioder i nivån ska visas. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Ställer in tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån. Standardvärdet är [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | tidslinjeenhet [TimescaleUnit](../../com.aspose.tasks/timescaleunit) för tidslinjenivån. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Ställer in ett värde som anger om nivåetiketterna ska baseras på räkenskapsåret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om nivåetiketterna ska baseras på räkenskapsåret. |

