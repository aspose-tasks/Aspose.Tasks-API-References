---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API-referens"
description: "Signaliserar till en CancellationToken att den ska avbrytas."
type: docs
weight: 47
url: /sv/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Signaliserar till en `CancellationToken` att den ska avbrytas.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [cancel()](#cancel--) | Kommunicerar en begäran om avbrytning. |
| [getToken()](#getToken--) | Skapar den nya `CancellationToken` som är associerad med denna `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | Hämtar om avbrytning har begärts för denna CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Kommunicerar en begäran om avbrytning.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Skapar den nya `CancellationToken` som är associerad med denna `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Hämtar om avbrytning har begärts för denna CancellationTokenSource.

**Returns:**
boolean - true, om avbrytning har begärts; false annars.
