---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een enkele laag van de tijdschaal op een Gantt-diagram voor."
type: docs
weight: 325
url: /nl/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Stelt een enkele laag van de tijdschaal op een Gantt-diagram voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Initialiseert een nieuw exemplaar van de klasse [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Initialiseert een nieuw exemplaar van de klasse [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAlignment()](#getAlignment--) | Haalt op hoe labels binnen elke tijdsperiode van de tier uitgelijnd moeten worden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Haalt het tijdseenheid-interval op waarin labels voor de tier worden weergegeven. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Haalt een callback-functie op voor het afhandelen van het renderen van datum-ticks in deze tier. |
| [getLabel()](#getLabel--) | Haalt het datumlabel [DateLabel](../../com.aspose.tasks/datelabel) op voor de timescale tier. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Haalt de vlag op die bepaalt of datumlabels op elke pagina moeten worden gerenderd wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. |
| [getShowTicks()](#getShowTicks--) | Haalt een waarde op die aangeeft of tickmarks die tijdsperioden in de tier scheiden, moeten worden weergegeven. |
| [getUnit()](#getUnit--) | Haalt de timescale-eenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) op voor de timescale tier. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Haalt een waarde op die aangeeft of de tier-labels gebaseerd moeten worden op het fiscale jaar. |
| [setAlignment(int value)](#setAlignment-int-) | Stelt in hoe labels binnen elke tijdsperiode van de tier uitgelijnd moeten worden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Stelt het tijdseenheid-interval in waarin labels voor de tier worden weergegeven. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Stelt een callback-functie in voor het afhandelen van het renderen van datum-ticks in deze tier. |
| [setLabel(int value)](#setLabel-int-) | Stelt het datumlabel [DateLabel](../../com.aspose.tasks/datelabel) in voor de timescale tier. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Stelt de vlag in die bepaalt of datumlabels op elke pagina moeten worden gerenderd wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Stelt een waarde in die aangeeft of tickmarks die tijdsperioden in de tier scheiden, moeten worden weergegeven. |
| [setUnit(int value)](#setUnit-int-) | Stelt de timescale-eenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) in voor de timescale tier. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Stelt een waarde in die aangeeft of de tier-labels gebaseerd moeten worden op het fiscale jaar. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Initialiseert een nieuw exemplaar van de klasse [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Initialiseert een nieuw exemplaar van de klasse [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| unit | int | De timescale-eenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Het aantal [TimescaleUnit](../../com.aspose.tasks/timescaleunit)-eenheden. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Haalt op hoe labels binnen elke tijdsperiode van de tier uitgelijnd moeten worden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - hoe labels binnen elke tijdsperiode van de tier uitgelijnd moeten worden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Haalt het tijdseenheid-interval op waarin labels voor de tier worden weergegeven. De standaardwaarde is 1.

**Returns:**
int - het tijdseenheid-interval waarin labels voor de tier worden weergegeven.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Haalt een callback-functie op voor het afhandelen van het renderen van datum-ticks in deze tier.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Haalt het datumlabel [DateLabel](../../com.aspose.tasks/datelabel) op voor de timescale tier.

**Returns:**
int - datumlabel [DateLabel](../../com.aspose.tasks/datelabel) voor de timescale tier.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Haalt de vlag op die bepaalt of datumlabels op elke pagina moeten worden gerenderd wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. Als de waarde 'true' is, worden datumlabels voor de periode op elke pagina gerenderd wanneer de tijdsperiode zich over meerdere pagina's uitstrekt. Als de waarde 'false' is, wordt het datumlabel slechts één keer gerenderd volgens de waarde van `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) eigenschap.

--------------------

Heeft geen equivalent in MS Project.

**Returns:**
boolean - vlag die bepaalt of datummarkeringen op elke pagina moeten worden weergegeven wanneer een tijdsperiode zich over meerdere pagina's uitstrekt.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Haalt een waarde op die aangeeft of tickmarks die tijdsperioden in de tier scheiden, moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of er markeringen moeten worden getoond die tijdsperioden in de laag scheiden.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Haalt de tijdschaaleenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) op voor de tijdschaallaag. De standaardwaarde is [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - tijdschaaleenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) voor de tijdschaallaag.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Haalt een waarde op die aangeeft of de tier-labels gebaseerd moeten worden op het fiscale jaar.

**Returns:**
boolean - een waarde die aangeeft of de laaglabels gebaseerd moeten zijn op het fiscale jaar.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Stelt in hoe labels binnen elke tijdsperiode van de tier uitgelijnd moeten worden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | hoe labels uit te lijnen binnen elke tijdsperiode van de laag ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Stelt het tijdseenheidsinterval in waarin labels voor de laag worden weergegeven. De standaardwaarde is 1.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het tijdseenheidsinterval waarin labels voor de laag worden weergegeven. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Stelt een callback-functie in voor het afhandelen van het renderen van datum-ticks in deze tier.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | een callback-functie voor het afhandelen van het renderen van datumstippen in deze laag. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Stelt het datumlabel [DateLabel](../../com.aspose.tasks/datelabel) in voor de timescale tier.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | datummarkering [DateLabel](../../com.aspose.tasks/datelabel) voor de tijdschaallaag. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Stelt de vlag in die bepaalt of datummarkeringen op elke pagina moeten worden weergegeven wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. Als de waarde 'true' is, worden de datummarkeringen voor de periode op elke pagina weergegeven. Als de waarde 'false' is, wordt de datummarkering slechts één keer weergegeven volgens de waarde van `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) eigenschap.

--------------------

Heeft geen equivalent in MS Project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | vlag die bepaalt of datummarkeringen op elke pagina moeten worden weergegeven wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Stelt een waarde in die aangeeft of tickmarks die tijdsperioden in de tier scheiden, moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of er markeringen moeten worden getoond die tijdsperioden in de laag scheiden. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Stelt de tijdschaaleenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) in voor de tijdschaallaag. De standaardwaarde is [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | tijdschaaleenheid [TimescaleUnit](../../com.aspose.tasks/timescaleunit) voor de tijdschaallaag. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Stelt een waarde in die aangeeft of de tier-labels gebaseerd moeten worden op het fiscale jaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de laaglabels gebaseerd moeten worden op het fiscale jaar. |

