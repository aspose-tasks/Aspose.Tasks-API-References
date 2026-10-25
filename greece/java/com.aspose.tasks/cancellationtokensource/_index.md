---
title: "CancellationTokenSource"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Σηματοδοτεί σε ένα CancellationToken ότι πρέπει να ακυρωθεί."
type: docs
weight: 47
url: /el/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Σηματοδοτεί σε ένα `CancellationToken` ότι πρέπει να ακυρωθεί.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [cancel()](#cancel--) | Μεταδίδει ένα αίτημα ακύρωσης. |
| [getToken()](#getToken--) | Δημιουργεί το νέο `CancellationToken` που συσχετίζεται με αυτό το `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | Λαμβάνει αν έχει ζητηθεί ακύρωση για αυτό το CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Μεταδίδει ένα αίτημα ακύρωσης.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Δημιουργεί το νέο `CancellationToken` που συσχετίζεται με αυτό το `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Λαμβάνει αν έχει ζητηθεί ακύρωση για αυτό το CancellationTokenSource.

**Returns:**
boolean - true, εάν έχει ζητηθεί ακύρωση· false διαφορετικά.
