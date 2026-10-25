---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un callback che viene chiamato quando ogni pagina di un documento multipagina viene salvata in un flusso separato."
type: docs
weight: 382
url: /it/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Rappresenta un callback che viene chiamato quando ogni pagina di un documento multipagina viene salvata in un flusso separato.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [onFinish()](#onFinish--) | Metodo che verrà chiamato quando tutte le pagine sono state scritte. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Il metodo da chiamare quando una pagina viene salvata in uno stream. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Metodo che verrà chiamato quando tutte le pagine sono state scritte.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Il metodo da chiamare quando una pagina viene salvata in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Gli argomenti di salvataggio della pagina. |

