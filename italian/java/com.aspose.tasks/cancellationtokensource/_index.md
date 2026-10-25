---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API Reference"
description: "Segnala a un CancellationToken che deve essere annullato."
type: docs
weight: 47
url: /it/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Invia un segnale a un `CancellationToken` che dovrebbe essere annullato.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [cancel()](#cancel--) | Comunica una richiesta di annullamento. |
| [getToken()](#getToken--) | Crea il nuovo `CancellationToken` associato a questo `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | Ottiene se è stata richiesta l'annullamento per questo CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Comunica una richiesta di annullamento.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Crea il nuovo `CancellationToken` associato a questo `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Ottiene se è stata richiesta l'annullamento per questo CancellationTokenSource.

**Returns:**
boolean - true, se è stata richiesta l'annullamento; false altrimenti.
