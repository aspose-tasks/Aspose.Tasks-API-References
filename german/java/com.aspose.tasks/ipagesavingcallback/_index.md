---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Callback dar, der aufgerufen wird, wenn jede Seite in einem mehrseitigen Dokument in einen separaten Stream gespeichert wird."
type: docs
weight: 382
url: /de/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Stellt einen Callback dar, der aufgerufen wird, wenn jede Seite in einem mehrseitigen Dokument in einen separaten Stream gespeichert wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [onFinish()](#onFinish--) | Methode, die aufgerufen wird, wenn alle Seiten geschrieben wurden. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Die Methode, die aufgerufen wird, wenn eine Seite in einen Stream gespeichert wird. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Methode, die aufgerufen wird, wenn alle Seiten geschrieben wurden.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Die Methode, die aufgerufen wird, wenn eine Seite in einen Stream gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Die Argumente zum Speichern der Seite. |

