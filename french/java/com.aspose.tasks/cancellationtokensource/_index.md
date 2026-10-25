---
title: "CancellationTokenSource"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Signale à un CancellationToken qu'il doit être annulé."
type: docs
weight: 47
url: /fr/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Signale à un `CancellationToken` qu'il doit être annulé.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [cancel()](#cancel--) | Communique une demande d'annulation. |
| [getToken()](#getToken--) | Crée le nouveau `CancellationToken` associé à ce `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | Obtient si une annulation a été demandée pour ce CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Communique une demande d'annulation.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Crée le nouveau `CancellationToken` associé à ce `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Obtient si une annulation a été demandée pour ce CancellationTokenSource.

**Returns:**
booléen - true, si une annulation a été demandée ; false sinon.
