---
title: "FontSettings.FontResolveCallback"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété FontSettings. Obtient ou définit un rappel qui peut être utilisé pour personnaliser les polices résolues"
type: docs
weight: 30
url: /fr/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

Obtient ou définit un rappel qui peut être utilisé pour personnaliser les polices résolues.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## Exemples

Montre comment définir un rappel de résolution de police personnalisé pour exécuter du code défini par l'utilisateur afin de définir une police de secours ou de substituer la police spécifique.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // Il semble que la police exacte ne puisse pas être trouvée et qu'une police de secours a été définie.
        // Nous pouvons remplacer la police de secours.
        args.ResolvedFontName = "Arial";
    }

    // Ou simplement substituer la police spécifique :
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Voir aussi

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


