---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks für .NET-API-Referenz
description: TaskLinkCollection methode. Gibt eine Instanz von FinishStart zurückTaskLink die dem TaskLinkCollectionObjekt hinzugefügt wurde.
type: docs
weight: 40
url: /de/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Gibt eine Instanz von Finish-Start zurück[`TaskLink`](../../tasklink/) die dem TaskLinkCollection-Objekt hinzugefügt wurde.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | Task | Vorgängeraufgabe. |
| succ | Task | Nachfolgeaufgabe. |

### Rückgabewert

eine Task-Link-Instanz, die diesem Objekt hinzugefügt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wenn eine der Eingabeaufgaben gleich null ist, dannArgumentNullException wird geworfen. |

### Siehe auch

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namensraum [Aspose.Tasks](../../tasklinkcollection/)
* Montage [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Gibt eine Instanz von zurück[`TaskLink`](../../tasklink/) die dem TaskLinkCollection-Objekt hinzugefügt wurde.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | Task | Vorgängeraufgabe. |
| succ | Task | Nachfolgeaufgabe. |
| linkType | TaskLinkType | Linktyp[`TaskLinkType`](../../tasklinktype/) |

### Rückgabewert

eine Task-Link-Instanz, die diesem Objekt hinzugefügt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wenn eine der Eingabeaufgaben gleich null ist, dannArgumentNullException wird geworfen. |

### Siehe auch

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namensraum [Aspose.Tasks](../../tasklinkcollection/)
* Montage [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Gibt eine Instanz von zurück[`TaskLink`](../../tasklink/) die dem TaskLinkCollection-Objekt hinzugefügt wurde.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | Task | Vorgängeraufgabe. |
| succ | Task | Nachfolgeaufgabe. |
| linkType | TaskLinkType | Linktyp[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Verbindungsverzögerung[`Duration`](../../duration/). |

### Rückgabewert

eine Aufgabenverknüpfung, die diesem Objekt hinzugefügt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wenn eine der Eingabeaufgaben gleich null ist, dannArgumentNullException wird geworfen. |

### Siehe auch

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namensraum [Aspose.Tasks](../../tasklinkcollection/)
* Montage [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Dies ist die Stub-Implementierung der Add-Methode von ICollection, die nur NotSupportedException auslöst.

```csharp
public void Add(TaskLink item)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | TaskLink | Das hinzuzufügende Element. |

### Siehe auch

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namensraum [Aspose.Tasks](../../tasklinkcollection/)
* Montage [Aspose.Tasks](../../../)


