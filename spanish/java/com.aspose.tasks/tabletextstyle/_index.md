---
title: "TableTextStyle"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un estilo de texto en una tabla de vista."
type: docs
weight: 288
url: /es/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Representa un estilo de texto en una tabla de vista.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la fuente especificada. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con el tamaño de fuente y el estilo de fuente especificados. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la configuración de fuente predeterminada y el estilo de fuente especificado. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getField()](#getField--) | Obtiene un campo al que se aplicará el estilo. |
| [getItemType()](#getItemType--) | Devuelve el tipo de elemento de texto. |
| [getRowUid()](#getRowUid--) | Obtiene un identificador único de fila. |
| [setField(int value)](#setField-int-) | Establece un campo al que se aplicará el estilo. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | int | Un identificador único de fila especificado. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la fuente especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | int | Un identificador único de fila especificado. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Una fuente sobre la cual se basa un estilo de texto. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con el tamaño de fuente y el estilo de fuente especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | int | Un identificador único de fila especificado. |
| fontSize | float | Tamaño de una fuente en la que se basa un estilo de texto. |
| fontStyle | int | Estilo de fuente. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Inicializa una nueva instancia de la clase [TableTextStyle](../../com.aspose.tasks/tabletextstyle) con la configuración de fuente predeterminada y el estilo de fuente especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | int | Un identificador único de fila especificado. |
| fontStyle | int | Estilo de fuente. |

### getField() {#getField--}
```
public final int getField()
```


Obtiene un campo al que se aplicará el estilo. `Field`([getField()](../../com.aspose/tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - un campo al que se aplicará el estilo.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Devuelve el tipo de elemento de texto.

**Returns:**
int - valor del tipo enumerado TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Obtiene un identificador único de fila.

--------------------

Devuelve -1 si el estilo se aplicará a todas las filas de una vista.

**Returns:**
int - un identificador único de fila.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Establece un campo al que se aplicará el estilo. `Field`([getField()](../../com.aspose/tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un campo al que se aplicará el estilo. |

