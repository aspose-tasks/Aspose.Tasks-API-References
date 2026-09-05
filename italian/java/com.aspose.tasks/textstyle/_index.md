---
title: "TextStyle"
second_title: "Aspose.Tasks for Java API Reference"
description: "Modifica lo stile visivo del testo per un elemento nella vista del progetto."
type: docs
weight: 315
url: /it/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

Modifica lo stile visivo del testo per un elemento nella vista del progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TextStyle()](#TextStyle--) | Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con le impostazioni predefinite. |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con il font predefinito e le dimensioni e lo stile del font specificati. |
| [TextStyle(int fontStyle)](#TextStyle-int-) | Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con il font predefinito e lo stile del font specificato. |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con le impostazioni del font specificate. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | Ottiene il colore di sfondo dello stile di testo. |
| [getBackgroundPattern()](#getBackgroundPattern--) | Ottiene il motivo di sfondo dello stile di testo. |
| [getColor()](#getColor--) | Ottiene il colore del testo. |
| [getFont()](#getFont--) | Ottiene il font dello stile di testo. |
| [getItemType()](#getItemType--) | Ottiene il [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Imposta il colore di sfondo dello stile di testo. |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | Imposta il motivo di sfondo dello stile di testo. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Imposta il colore del testo. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Imposta il font dello stile di testo. |
| [setItemType(int value)](#setItemType-int-) | Imposta il [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con le impostazioni predefinite.

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con il font predefinito e le dimensioni e lo stile del font specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontSize | float | Dimensione del carattere di TextStyle. |
| fontStyle | int | Stile del carattere di TextStyle. |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con il font predefinito e lo stile del font specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontStyle | int | Stile del carattere da applicare al carattere predefinito. |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


Inizializza una nuova istanza della classe [TextStyle](../../com.aspose.tasks/textstyle) con le impostazioni del font specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Carattere di TextStyle. |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Ottiene il colore di sfondo dello stile di testo. `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose/tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - colore di sfondo dello stile di testo.
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


Ottiene il modello di sfondo dello stile di testo. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose/tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - modello di sfondo dello stile di testo.
### getColor() {#getColor--}
```
public final Color getColor()
```


Ottiene il colore del testo.

**Returns:**
java.awt.Color - colore del testo.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Ottiene il font dello stile di testo.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Ottiene il [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo.

**Returns:**
int - [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo.
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Imposta il colore di sfondo dello stile di testo. `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose/tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color | colore di sfondo dello stile di testo. |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


Imposta il modello di sfondo dello stile di testo. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose/tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | modello di sfondo dello stile di testo. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


Imposta il colore del testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color | colore del testo. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Imposta il font dello stile di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | carattere dello stile di testo. |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


Imposta il [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | [TextItemType](../../com.aspose.tasks/textitemtype) dello stile di testo. |

