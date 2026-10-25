---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un singolo livello della scala temporale in un diagramma Gantt."
type: docs
weight: 325
url: /it/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Rappresenta un singolo livello della scala temporale in un diagramma Gantt.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Inizializza una nuova istanza della classe [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Inizializza una nuova istanza della classe [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAlignment()](#getAlignment--) | Ottiene come allineare le etichette all'interno di ogni periodo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Ottiene l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Ottiene una funzione di callback per gestire il rendering del tick di data in questo livello. |
| [getLabel()](#getLabel--) | Ottiene l'etichetta data [DateLabel](../../com.aspose.tasks/datelabel) per il livello della scala temporale. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Ottiene il flag che definisce se le etichette data devono essere renderizzate su ogni pagina quando un periodo di tempo si estende su più pagine. |
| [getShowTicks()](#getShowTicks--) | Ottiene un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello. |
| [getUnit()](#getUnit--) | Ottiene l'unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello della scala temporale. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Ottiene un valore che indica se basare le etichette del livello sull'anno fiscale. |
| [setAlignment(int value)](#setAlignment-int-) | Imposta come allineare le etichette all'interno di ogni periodo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Imposta l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Imposta una funzione di callback per gestire il rendering del tick di data in questo livello. |
| [setLabel(int value)](#setLabel-int-) | Imposta l'etichetta data [DateLabel](../../com.aspose.tasks/datelabel) per il livello della scala temporale. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Imposta il flag che definisce se le etichette data devono essere renderizzate su ogni pagina quando un periodo di tempo si estende su più pagine. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Imposta un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello. |
| [setUnit(int value)](#setUnit-int-) | Imposta l'unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello della scala temporale. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Imposta un valore che indica se basare le etichette del livello sull'anno fiscale. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Inizializza una nuova istanza della classe [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Inizializza una nuova istanza della classe [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| unit | int | L'unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Il conteggio delle unità [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Ottiene come allineare le etichette all'interno di ogni periodo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - come allineare le etichette all'interno di ogni periodo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Ottiene l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. Il valore predefinito è 1.

**Returns:**
int - l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Ottiene una funzione di callback per gestire il rendering del tick di data in questo livello.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Ottiene l'etichetta data [DateLabel](../../com.aspose.tasks/datelabel) per il livello della scala temporale.

**Returns:**
int - etichetta data [DateLabel](../../com.aspose.tasks/datelabel) per il livello della scala temporale.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Ottiene il flag che definisce se le etichette data devono essere renderizzate su ogni pagina quando un periodo di tempo si estende su più pagine. Se il valore è 'true', quando il periodo di tempo si estende su più pagine, le etichette data per il periodo sono renderizzate su ogni pagina. Se il valore è 'false', l'etichetta data è renderizzata una sola volta in base al valore della proprietà `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

Non ha l'equivalente in MS Project.

**Returns:**
boolean - flag che definisce se le etichette di data devono essere renderizzate su ogni pagina quando un intervallo di tempo si estende su più pagine.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Ottiene un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello.

**Returns:**
boolean - valore che indica se mostrare i segni di spunta che separano gli intervalli di tempo nel livello.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Ottiene l'unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello di scala temporale. Il valore predefinito è [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello di scala temporale.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Ottiene un valore che indica se basare le etichette del livello sull'anno fiscale.

**Returns:**
boolean - valore che indica se basare le etichette del livello sull'anno fiscale.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Imposta come allineare le etichette all'interno di ogni periodo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | come allineare le etichette all'interno di ciascun intervallo di tempo del livello ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Imposta l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. Il valore predefinito è 1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Imposta una funzione di callback per gestire il rendering del tick di data in questo livello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | una funzione di callback per gestire il rendering del segno di data in questo livello. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Imposta l'etichetta data [DateLabel](../../com.aspose.tasks/datelabel) per il livello della scala temporale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | etichetta di data [DateLabel](../../com.aspose.tasks/datelabel) per il livello di scala temporale. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Imposta il flag che definisce se le etichette di data devono essere renderizzate su ogni pagina quando un intervallo di tempo si estende su più pagine. Se il valore è 'true', quando l'intervallo di tempo si estende su più pagine, le etichette di data per il periodo sono renderizzate su ogni pagina. Se il valore è 'false', l'etichetta di data è renderizzata una sola volta in base al valore della proprietà `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

Non ha l'equivalente in MS Project.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | flag che definisce se le etichette di data devono essere renderizzate su ogni pagina quando un intervallo di tempo si estende su più pagine. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Imposta un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | valore che indica se mostrare i segni di spunta che separano gli intervalli di tempo nel livello. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Imposta l'unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello di scala temporale. Il valore predefinito è [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | unità di scala temporale [TimescaleUnit](../../com.aspose.tasks/timescaleunit) per il livello di scala temporale. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Imposta un valore che indica se basare le etichette del livello sull'anno fiscale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | valore che indica se basare le etichette del livello sull'anno fiscale. |

