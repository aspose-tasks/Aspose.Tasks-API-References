---
title: "TimescaleTier"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un nivel único de la escala de tiempo en un Diagrama de Gantt."
type: docs
weight: 325
url: /es/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Representa un nivel único de la escala de tiempo en un Diagrama de Gantt.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Inicializa una nueva instancia de la clase [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Inicializa una nueva instancia de la clase [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAlignment()](#getAlignment--) | Obtiene cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Obtiene el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Obtiene una función de devolución de llamada para manejar el renderizado de la marca de fecha en este nivel. |
| [getLabel()](#getLabel--) | Obtiene la etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Obtiene la bandera que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. |
| [getShowTicks()](#getShowTicks--) | Obtiene un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel. |
| [getUnit()](#getUnit--) | Obtiene la unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Obtiene un valor que indica si las etiquetas del nivel deben basarse en el año fiscal. |
| [setAlignment(int value)](#setAlignment-int-) | Establece cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Establece el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Establece una función de devolución de llamada para manejar el renderizado de la marca de fecha en este nivel. |
| [setLabel(int value)](#setLabel-int-) | Establece la etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Establece la bandera que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Establece un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel. |
| [setUnit(int value)](#setUnit-int-) | Establece la unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Establece un valor que indica si las etiquetas del nivel deben basarse en el año fiscal. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Inicializa una nueva instancia de la clase [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Inicializa una nueva instancia de la clase [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| unit | int | La unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | El recuento de unidades [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Obtiene cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Obtiene el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel. El valor predeterminado es 1.

**Returns:**
int - el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Obtiene una función de devolución de llamada para manejar el renderizado de la marca de fecha en este nivel.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Obtiene la etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo.

**Returns:**
int - etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Obtiene la bandera que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. Si el valor es 'true', cuando el período de tiempo abarca varias páginas, las etiquetas de fecha para el período se renderizan en cada página. Si el valor es 'false', la etiqueta de fecha se renderiza solo una vez según un valor de `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) propiedad.

--------------------

No tiene el equivalente en MS Project.

**Returns:**
boolean - indicador que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Obtiene un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel.

**Returns:**
boolean - un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Obtiene la unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo. El valor predeterminado es [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Obtiene un valor que indica si las etiquetas del nivel deben basarse en el año fiscal.

**Returns:**
boolean - un valor que indica si las etiquetas del nivel se basan en el año fiscal.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Establece cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Establece el intervalo de unidad de tiempo en el que se mostrarán las etiquetas para el nivel. El valor predeterminado es 1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el intervalo de unidad de tiempo en el que se mostrarán las etiquetas para el nivel. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Establece una función de devolución de llamada para manejar el renderizado de la marca de fecha en este nivel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | una función de devolución de llamada para manejar el renderizado de la marca de fecha en este nivel. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Establece la etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | etiqueta de fecha [DateLabel](../../com.aspose.tasks/datelabel) para el nivel de escala de tiempo. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Establece el indicador que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. Si el valor es 'true', cuando el período de tiempo abarca varias páginas, las etiquetas de fecha para el período se renderizan en cada página. Si el valor es 'false', la etiqueta de fecha se renderiza solo una vez según el valor de la propiedad `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

No tiene el equivalente en MS Project.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | indicador que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Establece un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben mostrar marcas de división que separan los períodos de tiempo en el nivel. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Establece la unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo. El valor predeterminado es [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | unidad de escala de tiempo [TimescaleUnit](../../com.aspose.tasks/timescaleunit) para el nivel de escala de tiempo. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Establece un valor que indica si las etiquetas del nivel deben basarse en el año fiscal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las etiquetas del nivel se basan en el año fiscal. |

