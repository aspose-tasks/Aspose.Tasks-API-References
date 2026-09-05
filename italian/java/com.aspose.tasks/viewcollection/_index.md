---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Contiene un elenco di oggetti."
type: docs
weight: 343
url: /it/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Contiene un elenco di oggetti [View](../../com.aspose.tasks/view). Estende la classe `AbstractCollection`.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Aggiunge l'elemento specificato a questa raccolta. |
| [clear()](#clear--) | Rimuove tutti gli elementi da questa collezione. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Restituisce true se l'elemento specificato è trovato in questa collezione; altrimenti, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Copia gli elementi di questa collezione nell'array specificato, iniziando dall'indice dell'array specificato. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Cerca una View con il nome e restituisce la prima occorrenza nella collezione. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Cerca una View con la proprietà Screen specificata e restituisce la prima occorrenza nella collezione. |
| [getParentProject()](#getParentProject--) | Ottiene il genitore dell'oggetto View. |
| [iterator()](#iterator--) | Restituisce un iteratore sugli elementi contenuti in questa collezione. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [size()](#size--) | Ottiene il numero di elementi contenuti in questa raccolta. |
| [toList()](#toList--) | Converte una collezione di viste in un elenco di oggetti [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Aggiunge l'elemento specificato a questa raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'elemento specificato da aggiungere a questa raccolta. |

**Returns:**
boolean - true se l'operazione è riuscita.
### clear() {#clear--}
```
public final void clear()
```


Rimuove tutti gli elementi da questa collezione.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Restituisce true se l'elemento specificato è trovato in questa collezione; altrimenti, false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'elemento specificato da trovare. |

**Returns:**
boolean - true se l'elemento specificato è trovato in questa collezione; altrimenti, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Copia gli elementi di questa collezione nell'array specificato, iniziando dall'indice dell'array specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | l'array monodimensionale specificato in cui copiare gli elementi |
| arrayIndex | int | l'indice basato su zero dell'array specificato a partire dal quale inizia la copia. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Cerca una View con il nome e restituisce la prima occorrenza nella collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| viewName | java.lang.String | Nome della View da cercare. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Cerca una View con la proprietà Screen specificata e restituisce la prima occorrenza nella collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| screen | int | Valore di enumerazione [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il genitore dell'oggetto View. Solo lettura [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Restituisce un iteratore sugli elementi contenuti in questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - iteratore della collezione.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Rimuove la prima occorrenza di un oggetto specifico da questa collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'oggetto specificato da rimuovere. |

**Returns:**
boolean - true se l'oggetto specificato è stato rimosso con successo da questa collezione; altrimenti, false.
### size() {#size--}
```
public final int size()
```


Ottiene il numero di elementi contenuti in questa raccolta.

**Returns:**
int - il numero di elementi contenuti in questa raccolta.
### toList() {#toList--}
```
public final List<View> toList()
```


Converte una collezione di viste in un elenco di oggetti [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Elenco generico di oggetti [View](../../com.aspose.tasks/view).
