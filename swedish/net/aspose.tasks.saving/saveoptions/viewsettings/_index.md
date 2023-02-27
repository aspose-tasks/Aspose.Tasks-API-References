---
title: SaveOptions.ViewSettings
second_title: Aspose.Tasks för .NET API-referens
description: SaveOptions fast egendom. Hämtar eller ställer in en vy View  att återge. Du kan använda de här alternativen för att uttryckligen ange vilken vy som ska sparas i PDF HTML eller bildformat. Om den här egenskapen är inställdPresentationFormat egenskapen ignoreras när projektet sparas. Vyn ska vara från en av följande skärmar Screen  Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage
type: docs
weight: 240
url: /sv/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Hämtar eller ställer in en vy ([`View`](../view/) ) att återge. Du kan använda de här alternativen för att uttryckligen ange vilken vy som ska sparas i PDF-, HTML- eller bildformat. Om den här egenskapen är inställd,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) egenskapen ignoreras när projektet sparas. Vyn ska vara från en av följande skärmar (([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | När set-metoden anropas och instans av View-klassen med ett värde som inte stöds av Screen-egenskapen tillhandahålls. |

### Se även

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namnutrymme [Aspose.Tasks.Saving](../../saveoptions/)
* hopsättning [Aspose.Tasks](../../../)


