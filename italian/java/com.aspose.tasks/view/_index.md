---
title: "View"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una vista in Project."
type: docs
weight: 342
url: /it/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Rappresenta una vista in Project.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [View()](#View--) | Inizializza una nuova istanza della classe [View](../../com.aspose/tasks/view). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Confronta l'istanza corrente con un altro oggetto dello stesso tipo e restituisce un intero che indica se l'istanza corrente precede, segue o si trova nella stessa posizione nell'ordine di ordinamento rispetto all'altro oggetto. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Crea una nuova istanza della classe [View](../../com.aspose/tasks/view). |
| [getFilter()](#getFilter--) | Ottiene un filtro utilizzato in una singola visualizzazione. |
| [getGroup()](#getGroup--) | Ottiene un gruppo della singola visualizzazione. |
| [getHighlightFilter()](#getHighlightFilter--) | Ottiene un valore che indica se Microsoft Project evidenzia il filtro per una singola visualizzazione. |
| [getName()](#getName--) | Ottiene il nome di un oggetto View. |
| [getPageInfo()](#getPageInfo--) | Ottiene un'istanza della classe `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Ottiene il genitore dell'oggetto View. |
| [getScreen()](#getScreen--) | Ottiene il tipo di schermo per la singola visualizzazione. |
| [getShowInMenu()](#getShowInMenu--) | Ottiene un valore che indica se Microsoft Project mostra il nome della singola visualizzazione nella lista a discesa View o Altre Visualizzazioni nel Ribbon. |
| [getTable()](#getTable--) | Ottiene una tabella della singola visualizzazione. |
| [getType()](#getType--) | Ottiene il tipo di elemento nella vista singola, ad esempio attività o risorse. |
| [getUid()](#getUid--) | Ottiene l'identificatore univoco di una vista. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Ottiene una raccolta di oggetti che rappresentano la posizione e l'aspetto di [OleObject](../../com.aspose.tasks/oleobject) nella vista. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Imposta un filtro utilizzato nella vista singola. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Imposta un gruppo della vista singola. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Imposta un valore che indica se Microsoft Project evidenzia il filtro per una vista singola. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome di un oggetto View. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Imposta un valore che indica se Microsoft Project mostra il nome della vista singola nelle liste a discesa Vista o Altre viste nella barra multifunzione. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Imposta una tabella della vista singola. |
### View() {#View--}
```
public View()
```


Inizializza una nuova istanza della classe [View](../../com.aspose/tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Confronta l'istanza corrente con un altro oggetto dello stesso tipo e restituisce un intero che indica se l'istanza corrente precede, segue o si trova nella stessa posizione nell'ordine di ordinamento rispetto all'altro oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | l'oggetto View specificato con cui confrontare questa istanza. |

**Returns:**
int - Un intero a 32 bit con segno che indica l'ordine relativo degli oggetti confrontati. Il valore restituito ha i seguenti significati: Valore Significato Meno di zero Questa istanza precede `other` nell'ordine di ordinamento. Zero Questa istanza si trova nella stessa posizione nell'ordine di ordinamento di `other`. Maggiore di zero Questa istanza segue `other` nell'ordine di ordinamento.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'oggetto specificato è una View che ha lo stesso valore Uid di questa istanza; altrimenti, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Crea una nuova istanza della classe [View](../../com.aspose/tasks/view).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| viewScreen | int | Il tipo di schermo per il quale la vista può essere visualizzata. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Ottiene un filtro utilizzato in una singola visualizzazione.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Ottiene un gruppo della singola visualizzazione.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Ottiene un valore che indica se Microsoft Project evidenzia il filtro per una singola visualizzazione.

**Returns:**
boolean - un valore che indica se Microsoft Project evidenzia il filtro per una vista singola.
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome di un oggetto View.

**Returns:**
java.lang.String - il nome di un oggetto View.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Ottiene un'istanza della classe `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). Rappresenta i dati di impostazione della pagina presenti nel formato file mpp.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il genitore dell'oggetto View. Solo lettura [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Ottiene il tipo di schermo per la vista singola. Solo lettura [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - il tipo di schermo per la vista singola.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Ottiene un valore che indica se Microsoft Project mostra il nome della singola visualizzazione nella lista a discesa View o Altre Visualizzazioni nel Ribbon.

**Returns:**
boolean - un valore che indica se Microsoft Project mostra il nome della vista singola nelle liste a discesa Vista o Altre viste nella barra multifunzione.
### getTable() {#getTable--}
```
public final Table getTable()
```


Ottiene una tabella della singola visualizzazione.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Ottiene il tipo di elemento nella vista singola, ad esempio attività o risorse. Solo lettura [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - il tipo di elemento nella vista singola, ad esempio attività o risorse.
### getUid() {#getUid--}
```
public final int getUid()
```


Ottiene l'identificatore univoco di una vista.

**Returns:**
int - l'identificatore univoco di una vista.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Ottiene una raccolta di oggetti che rappresentano la posizione e l'aspetto di [OleObject](../../com.aspose.tasks/oleobject) nella vista.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - una raccolta di oggetti che rappresentano la posizione e l'aspetto di [OleObject](../../com.aspose.tasks/oleobject) nella vista.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La prima visualizzazione. |
| b | [View](../../com.aspose.tasks/view) | La seconda visualizzazione. |

**Returns:**
boolean - un valore che indica se questa istanza è uguale a un oggetto specificato
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La prima visualizzazione. |
| b | [View](../../com.aspose.tasks/view) | La seconda visualizzazione. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore di un oggetto specificato
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La prima visualizzazione. |
| b | [View](../../com.aspose.tasks/view) | La seconda visualizzazione. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La prima visualizzazione. |
| b | [View](../../com.aspose.tasks/view) | La seconda visualizzazione. |

**Returns:**
boolean - un valore che indica se questa istanza non è uguale a un oggetto specificato
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Restituisce un valore che indica se questa istanza è minore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Il primo filtro. |
| b | [View](../../com.aspose.tasks/view) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è minore di un oggetto specificato
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La prima visualizzazione. |
| b | [View](../../com.aspose.tasks/view) | La seconda visualizzazione. |

**Returns:**
boolean - un valore che indica se questa istanza è minore o uguale a un oggetto specificato
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Imposta un filtro utilizzato nella vista singola.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | un filtro utilizzato in una singola visualizzazione. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Imposta un gruppo della vista singola.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | un gruppo della singola visualizzazione. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Imposta un valore che indica se Microsoft Project evidenzia il filtro per una vista singola.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Microsoft Project evidenzia il filtro per una singola visualizzazione. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Imposta il nome di un oggetto View.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome di un oggetto View. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Imposta un valore che indica se Microsoft Project mostra il nome della vista singola nelle liste a discesa Vista o Altre viste nella barra multifunzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Microsoft Project mostra il nome della visualizzazione singola nella View o nelle liste a discesa Other Views nella Ribbon. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Imposta una tabella della vista singola.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | una tabella della visualizzazione singola. |

