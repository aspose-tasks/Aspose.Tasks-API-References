---
title: "PageSavingArgs"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Cette classe représente un ensemble de données liées à l'enregistrement d'une page de document dans un flux."
type: docs
weight: 180
url: /fr/java/com.aspose.tasks/pagesavingargs/
---

**Inheritance:**
java.lang.Object
```
public final class PageSavingArgs
```

Cette classe représente un ensemble de données liées à l'enregistrement de la page du document dans un flux.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Obtient une valeur indiquant si la routine de rendu doit garder le `Stream`([getStream()](../../com.aspose.tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose.tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après l'écriture d'une page. |
| [getPageNumber()](#getPageNumber--) | Obtient le numéro de la page à écrire. |
| [getStream()](#getStream--) | Obtient un flux pour écrire une page. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Définit une valeur indiquant si la routine de rendu doit conserver le `Stream`([getStream()](../../com.aspose/tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose/tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après qu'une page a été écrite. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Définit un flux pour écrire une page. |
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Obtient une valeur indiquant si la routine de rendu doit garder le `Stream`([getStream()](../../com.aspose.tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose.tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après l'écriture d'une page.

**Returns:**
boolean - une valeur indiquant si la routine de rendu doit conserver le `Stream`([getStream()](../../com.aspose/tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose/tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après qu'une page a été écrite.
### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Obtient le numéro de la page à écrire.

**Returns:**
int - un nombre de pages à écrire.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Obtient un flux pour écrire une page.

**Returns:**
java.io.OutputStream - un flux pour écrire une page.
### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Définit une valeur indiquant si la routine de rendu doit conserver le `Stream`([getStream()](../../com.aspose/tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose/tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après qu'une page a été écrite.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | boolean | une valeur indiquant si la routine de rendu doit conserver le `Stream`([getStream()](../../com.aspose/tasks/pagesavingargs\#getStream--)/[setStream(java.io.OutputStream)](../../com.aspose/tasks/pagesavingargs\#setStream-java.io.OutputStream-)) ouvert après qu'une page a été écrite. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Définit un flux pour écrire une page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.io.OutputStream | un flux pour écrire une page. |

