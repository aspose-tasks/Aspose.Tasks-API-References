---
title: "IPageSavingCallback"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una devolución de llamada que se invoca cuando cada página de un documento multipágina se guarda en un flujo separado."
type: docs
weight: 382
url: /es/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Representa una devolución de llamada que se invoca cuando cada página de un documento multipágina se guarda en un flujo separado.
## Métodos

| Método | Descripción |
| --- | --- |
| [onFinish()](#onFinish--) | Método que será llamado cuando se hayan escrito todas las páginas. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | El método que se llamará cuando una página se guarde en un flujo. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Método que será llamado cuando se hayan escrito todas las páginas.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


El método que se llamará cuando una página se guarde en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Los argumentos de guardado de la página. |

