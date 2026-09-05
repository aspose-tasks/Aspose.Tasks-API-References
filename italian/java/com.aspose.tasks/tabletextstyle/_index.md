---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta uno stile di testo in una tabella di visualizzazione."
type: docs
weight: 288
url: /it/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Rappresenta uno stile di testo in una tabella di visualizzazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con il font specificato. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la dimensione del font e lo stile del font specificati. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con le impostazioni predefinite del font e lo stile del font specificato. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getField()](#getField--) | Ottiene un campo a cui lo stile deve essere applicato. |
| [getItemType()](#getItemType--) | Restituisce il tipo di elemento di testo. |
| [getRowUid()](#getRowUid--) | Ottiene un ID univoco della riga. |
| [setField(int value)](#setField-int-) | Imposta un campo a cui lo stile deve essere applicato. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | int | Un ID univoco di riga specificato. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con il font specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | int | Un ID univoco di riga specificato. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Un font su cui si basa uno stile di testo. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la dimensione del font e lo stile del font specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | int | Un ID univoco di riga specificato. |
| fontSize | float | Dimensione di un font su cui si basa uno stile di testo. |
| fontStyle | int | Stile del font. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Inizializza una nuova istanza della classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con le impostazioni predefinite del font e lo stile del font specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | int | Un ID univoco di riga specificato. |
| fontStyle | int | Stile del font. |

### getField() {#getField--}
```
public final int getField()
```


Ottiene un campo a cui lo stile deve essere applicato. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - un campo a cui lo stile deve essere applicato.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Restituisce il tipo di elemento di testo.

**Returns:**
int - valore del tipo enumerato TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Ottiene un ID univoco della riga.

--------------------

Restituisce -1 se lo stile deve essere applicato a tutte le righe di una vista.

**Returns:**
int - un ID unico di riga.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Imposta un campo a cui lo stile deve essere applicato. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un campo a cui lo stile deve essere applicato. |

