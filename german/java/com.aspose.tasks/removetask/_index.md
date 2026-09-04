---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API Reference"
description: "Entfernt die angegebene Aufgabe aus einem Aufgabenbaum."
type: docs
weight: 246
url: /de/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Entfernt die angegebene Aufgabe aus einem Aufgabenbaum.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Initialisiert eine neue Instanz der [RemoveTask](../../com.aspose.tasks/removetask)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Nichts tun. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Nichts tun. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Entfernt die Aufgabe aus der angegebenen übergeordneten Aufgabe. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Initialisiert eine neue Instanz der [RemoveTask](../../com.aspose.tasks/removetask)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Zu entfernende Aufgabe. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Nichts tun.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Zu verarbeitendes Objekt. |
| Ebene | int | Baumknotenebene. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Nichts tun.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Zu verarbeitendes Objekt. |
| Ebene | int | Baumknotenebene. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Entfernt die Aufgabe aus der angegebenen übergeordneten Aufgabe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Übergeordnete Aufgabe. |
| Ebene | int | Baumknotenebene. |

