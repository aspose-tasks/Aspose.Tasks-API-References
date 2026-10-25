---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "MPPSaveOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob vorhandene VBA‑Makrodaten beim Speichern eines Projekts im MPP‑Format entfernt werden sollen."
type: docs
weight: 20
url: /de/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Gibt einen Wert zurück oder legt ihn fest, der angibt, ob vorhandene VBA‑Makrodaten beim Speichern eines Projekts im MPP‑Format entfernt werden sollen.

```csharp
public bool ClearVba { get; set; }
```

## Beispiele

Zeigt, wie VBA‑Makros aus einer MPP‑Datei entfernt werden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Siehe auch

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


