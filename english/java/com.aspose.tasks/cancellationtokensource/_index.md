---
title: CancellationTokenSource
second_title: Aspose.Tasks for Java API Reference
description: Signals to a CancellationToken that it should be canceled.
type: docs
weight: 47
url: /java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Signals to a CancellationToken that it should be canceled.
## Constructors

| Constructor | Description |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Methods

| Method | Description |
| --- | --- |
| [cancel()](#cancel--) | Communicates a request for cancellation. |
| [getToken()](#getToken--) | Creates the new CancellationToken associated with this CancellationTokenSource. |
| [isCancellationRequested()](#isCancellationRequested--) | Gets whether cancellation has been requested for this CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Communicates a request for cancellation.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Creates the new CancellationToken associated with this CancellationTokenSource.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this CancellationTokenSource.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Gets whether cancellation has been requested for this CancellationTokenSource.

**Returns:**
boolean - true, if cancellation has been requested; false otherwise.
