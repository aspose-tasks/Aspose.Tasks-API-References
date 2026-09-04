---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API Reference"
description: "Signalisiert einem CancellationToken, dass er abgebrochen werden soll."
type: docs
weight: 47
url: /de/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Signalisiert einem `CancellationToken`, dass er abgebrochen werden soll.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [cancel()](#cancel--) | Übermittelt eine Anforderung zum Abbruch. |
| [getToken()](#getToken--) | Erstellt das neue `CancellationToken`, das mit diesem `CancellationTokenSource` verknüpft ist. |
| [isCancellationRequested()](#isCancellationRequested--) | Ermittelt, ob für dieses CancellationTokenSource ein Abbruch angefordert wurde. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Übermittelt eine Anforderung zum Abbruch.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Erstellt das neue `CancellationToken`, das mit diesem `CancellationTokenSource` verknüpft ist.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Ermittelt, ob für dieses CancellationTokenSource ein Abbruch angefordert wurde.

**Returns:**
boolean – true, wenn ein Abbruch angefordert wurde; sonst false.
