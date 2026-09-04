---
title: "IPageSavingCallback"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un rappel qui est appelé lorsque chaque page d'un document multipage est enregistrée dans un flux séparé."
type: docs
weight: 382
url: /fr/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Représente un rappel qui est appelé lorsque chaque page d'un document multipage est enregistrée dans un flux séparé.
## Méthodes

| Méthode | Description |
| --- | --- |
| [onFinish()](#onFinish--) | Méthode qui sera appelée lorsque toutes les pages sont écrites. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | La méthode à appeler lorsqu'une page est enregistrée dans un flux. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Méthode qui sera appelée lorsque toutes les pages sont écrites.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


La méthode à appeler lorsqu'une page est enregistrée dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Les arguments de sauvegarde de la page. |

