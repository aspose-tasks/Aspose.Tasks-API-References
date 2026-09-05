---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta le impostazioni di stampa per una pagina della vista progetto."
type: docs
weight: 181
url: /it/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Rappresenta le impostazioni di stampa per una pagina della vista progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PageSettings()](#PageSettings--) | Inizializza una nuova istanza della classe [PageSettings](../../com.aspose.tasks/pagesettings). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Restituisce un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Restituisce il numero della prima pagina per la stampa. |
| [getPagesInHeight()](#getPagesInHeight--) | Restituisce il numero di pagine in altezza da stampare. |
| [getPagesInWidth()](#getPagesInWidth--) | Restituisce il numero di pagine in larghezza da stampare. |
| [getPaperSize()](#getPaperSize--) | Restituisce una dimensione della carta. |
| [getPaperSizeId()](#getPaperSizeId--) | Restituisce un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Restituisce una percentuale della dimensione normale a cui regolare la stampa. |
| [isPortrait()](#isPortrait--) | Restituisce un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Imposta un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Imposta il numero della prima pagina per la stampa. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Imposta il numero di pagine in altezza da stampare. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Imposta il numero di pagine in larghezza da stampare. |
| [setPaperSize(int value)](#setPaperSize-int-) | Imposta una dimensione della carta. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Imposta un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Imposta una percentuale della dimensione normale a cui regolare la stampa. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Inizializza una nuova istanza della classe [PageSettings](../../com.aspose/tasks/pagesettings). Rappresenta le impostazioni di stampa per una pagina della vista del progetto.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Restituisce un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale.

--------------------

Non è efficace quando il progetto è renderizzato in formato HTML.

**Returns:**
boolean - un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Restituisce il numero della prima pagina per la stampa.

**Returns:**
short - il numero della prima pagina per la stampa.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Restituisce il numero di pagine in altezza da stampare.

**Returns:**
int - il numero di pagine in altezza da stampare.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Restituisce il numero di pagine in larghezza da stampare.

**Returns:**
int - il numero di pagine in larghezza da stampare.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Restituisce una dimensione della carta. Può essere uno dei valori dell'enumerazione [PrinterPaperSize](../../com.aspose/tasks/printerpapersize).

**Returns:**
int - una dimensione della carta.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Restituisce un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato. Questo valore può essere usato per ottenere PaperSize dalle impostazioni del sistema operativo ().

**Returns:**
int - un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Restituisce una percentuale della dimensione normale a cui regolare la stampa.

**Returns:**
int - una percentuale della dimensione normale a cui regolare la stampa.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Restituisce un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

--------------------

È applicabile durante il rendering quando SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Imposta un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale.

--------------------

Non è efficace quando il progetto è renderizzato in formato HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | boolean | un valore che indica se regolare la stampa alla percentuale specificata (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) della dimensione normale. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Imposta il numero della prima pagina per la stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short | un numero di prima pagina per la stampa. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Imposta il numero di pagine in altezza da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di pagine in altezza da stampare. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Imposta il numero di pagine in larghezza da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di pagine in larghezza da stampare. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Imposta una dimensione carta. Può essere uno dei valori dell'enumerazione [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | una dimensione carta. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Imposta un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato. Questo valore può essere usato per ottenere PaperSize dalle impostazioni del sistema operativo ().

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzato. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Imposta una percentuale della dimensione normale a cui regolare la stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | una percentuale della dimensione normale a cui regolare la stampa. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

--------------------

È applicabile durante il rendering quando SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |

