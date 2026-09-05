---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Geeft een signaal aan een CancellationToken dat deze moet worden geannuleerd."
type: docs
weight: 47
url: /nl/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Geeft een signaal aan een `CancellationToken` dat deze geannuleerd moet worden.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [cancel()](#cancel--) | Communiceert een verzoek tot annulering. |
| [getToken()](#getToken--) | Maakt de nieuwe `CancellationToken` aan die aan deze `CancellationTokenSource` is gekoppeld. |
| [isCancellationRequested()](#isCancellationRequested--) | Haalt op of annulering is aangevraagd voor deze CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Communiceert een verzoek tot annulering.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Maakt de nieuwe `CancellationToken` aan die aan deze `CancellationTokenSource` is gekoppeld.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Haalt op of annulering is aangevraagd voor deze CancellationTokenSource.

**Returns:**
boolean - true, als annulering is aangevraagd; false anders.
