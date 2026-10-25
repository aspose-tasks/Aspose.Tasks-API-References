---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een callback voor die wordt aangeroepen wanneer elke pagina in een meerpagina-document wordt opgeslagen in een aparte stream."
type: docs
weight: 382
url: /nl/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Stelt een callback voor die wordt aangeroepen wanneer elke pagina in een meerpagina-document wordt opgeslagen in een aparte stream.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [onFinish()](#onFinish--) | Methode die wordt aangeroepen wanneer alle pagina's zijn geschreven. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | De methode die moet worden aangeroepen wanneer een pagina naar een stream wordt opgeslagen. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Methode die wordt aangeroepen wanneer alle pagina's zijn geschreven.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


De methode die moet worden aangeroepen wanneer een pagina naar een stream wordt opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | De argumenten voor het opslaan van de pagina. |

