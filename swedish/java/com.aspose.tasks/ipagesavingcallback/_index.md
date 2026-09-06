---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en återuppringning som anropas när varje sida i ett flersidigt dokument sparas till ett separat flöde."
type: docs
weight: 382
url: /sv/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Representerar en återuppringning som anropas när varje sida i ett flersidigt dokument sparas till ett separat flöde.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [onFinish()](#onFinish--) | Metod som kommer att anropas när alla sidor har skrivits. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Metoden som ska anropas när en sida sparas till en ström. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Metod som kommer att anropas när alla sidor har skrivits.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Metoden som ska anropas när en sida sparas till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Argumenten för sidsparning. |

