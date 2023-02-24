---
title: SaveOptions.ViewSettings
second_title: Aspose.Tasks für .NET-API-Referenz
description: SaveOptions eigendom. Ruft eine Ansicht ab oder legt sie fest View  zu rendern. Mit diesen Optionen können Sie explizit angeben welche Ansicht im PDF HTML oder Bildformat gespeichert werden soll. Wenn diese Eigenschaft gesetzt istPresentationFormat Die Eigenschaft wird beim Speichern des Projekts ignoriert. Die Ansicht sollte von einem der folgenden Bildschirme erfolgen Screen  Gantt Aufgabenblatt Aufgabennutzung Ressourcenblatt Ressourcennutzung
type: docs
weight: 240
url: /de/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Ruft eine Ansicht ab oder legt sie fest ([`View`](../view/) ) zu rendern. Mit diesen Optionen können Sie explizit angeben, welche Ansicht im PDF-, HTML- oder Bildformat gespeichert werden soll. Wenn diese Eigenschaft gesetzt ist,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) Die Eigenschaft wird beim Speichern des Projekts ignoriert. Die Ansicht sollte von einem der folgenden Bildschirme erfolgen (([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt, Aufgabenblatt, Aufgabennutzung, Ressourcenblatt, Ressourcennutzung)

```csharp
public View ViewSettings { get; set; }
```

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wenn die set-Methode aufgerufen wird und eine Instanz der View-Klasse mit einem nicht unterstützten Wert der Screen-Eigenschaft bereitgestellt wird. |

### Siehe auch

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namensraum [Aspose.Tasks.Saving](../../saveoptions/)
* Montage [Aspose.Tasks](../../../)


