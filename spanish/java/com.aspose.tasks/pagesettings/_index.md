---
title: "PageSettings"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa la configuración de impresión para una página de la vista del proyecto."
type: docs
weight: 181
url: /es/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Representa la configuración de impresión para una página de la vista del proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PageSettings()](#PageSettings--) | Inicializa una nueva instancia de la clase [PageSettings](../../com.aspose.tasks/pagesettings). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Obtiene un valor que indica si se debe ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Obtiene el número de la primera página para imprimir. |
| [getPagesInHeight()](#getPagesInHeight--) | Obtiene la cantidad de páginas en altura que se imprimirán. |
| [getPagesInWidth()](#getPagesInWidth--) | Obtiene la cantidad de páginas en anchura que se imprimirán. |
| [getPaperSize()](#getPaperSize--) | Obtiene un tamaño de papel. |
| [getPaperSizeId()](#getPaperSizeId--) | Obtiene un entero que representa uno de los valores de PrinterPaperSize o un identificador de tamaño de página personalizado. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Obtiene un porcentaje del tamaño normal al que se debe ajustar la impresión. |
| [isPortrait()](#isPortrait--) | Obtiene un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Establece un valor que indica si se debe ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Establece el número de la primera página para imprimir. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Establece la cantidad de páginas en altura que se imprimirán. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Establece la cantidad de páginas en anchura que se imprimirán. |
| [setPaperSize(int value)](#setPaperSize-int-) | Establece un tamaño de papel. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Establece un entero que representa uno de los valores de PrinterPaperSize o un identificador de tamaño de página personalizado. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Establece un porcentaje del tamaño normal al que se debe ajustar la impresión. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Inicializa una nueva instancia de la clase [PageSettings](../../com.aspose/tasks/pagesettings). Representa la configuración de impresión para una página de la vista del proyecto.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Obtiene un valor que indica si se debe ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal.

--------------------

No es efectivo cuando el proyecto se renderiza en formato HTML.

**Returns:**
boolean - un valor que indica si se debe ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Obtiene el número de la primera página para imprimir.

**Returns:**
short - el número de la primera página para imprimir.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Obtiene la cantidad de páginas en altura que se imprimirán.

**Returns:**
int - la cantidad de páginas en altura que se imprimirán.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Obtiene la cantidad de páginas en anchura que se imprimirán.

**Returns:**
int - la cantidad de páginas en anchura que se imprimirán.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Obtiene un tamaño de papel. Puede ser uno de los valores de la enumeración [PrinterPaperSize](../../com.aspose/tasks/printerpapersize).

**Returns:**
int - un tamaño de papel.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Obtiene un entero que representa uno de los valores de PrinterPaperSize o un identificador de tamaño de página personalizado. Este valor puede usarse para obtener PaperSize de la configuración del sistema operativo ().

**Returns:**
int - un entero que representa uno de los valores de PrinterPaperSize o un id de tamaño de página personalizado.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Obtiene un porcentaje del tamaño normal al que se debe ajustar la impresión.

**Returns:**
int - un porcentaje del tamaño normal al que ajustar la impresión.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Obtiene un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

--------------------

Se aplica durante el renderizado cuando SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Establece un valor que indica si se debe ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal.

--------------------

No es efectivo cuando el proyecto se renderiza en formato HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | boolean | un valor que indica si ajustar la impresión al porcentaje especificado (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) del tamaño normal. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Establece el número de la primera página para imprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short | un número de primera página para imprimir. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Establece la cantidad de páginas en altura que se imprimirán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de páginas en altura a imprimir. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Establece la cantidad de páginas en anchura que se imprimirán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de páginas en anchura a imprimir. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Establece un tamaño de papel. Puede ser uno de los valores de la enumeración [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un tamaño de papel. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Establece un entero que representa uno de los valores de PrinterPaperSize o un id de tamaño de página personalizado. Este valor puede usarse para obtener PaperSize de la configuración del SO ().

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un entero que representa uno de los valores de PrinterPaperSize o un id de tamaño de página personalizado. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Establece un porcentaje del tamaño normal al que se debe ajustar la impresión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un porcentaje del tamaño normal al que ajustar la impresión. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

--------------------

Se aplica durante el renderizado cuando SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |

