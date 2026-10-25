---
title: "CancellationTokenSource"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Indica a un CancellationToken que debe cancelarse."
type: docs
weight: 47
url: /es/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Envía una señal a un `CancellationToken` de que debe cancelarse.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [cancel()](#cancel--) | Comunica una solicitud de cancelación. |
| [getToken()](#getToken--) | Crea el nuevo `CancellationToken` asociado a este `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | Obtiene si se ha solicitado la cancelación para este CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Comunica una solicitud de cancelación.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Crea el nuevo `CancellationToken` asociado a este `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Obtiene si se ha solicitado la cancelación para este CancellationTokenSource.

**Returns:**
boolean - true, si se ha solicitado la cancelación; false en caso contrario.
