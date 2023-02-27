---
title: SaveOptions.ViewSettings
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: SaveOptions proprietà. Ottiene o imposta una vista View  rendere. Puoi utilizzare queste opzioni per specificare in modo esplicito quale vista deve essere salvata nei formati PDF HTML o Immagine. Se questa proprietà è impostataPresentationFormat proprietà viene ignorata quando il progetto viene salvato. La vista dovrebbe provenire da una delle seguenti schermate Screen  Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage
type: docs
weight: 240
url: /it/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Ottiene o imposta una vista ([`View`](../view/) ) rendere. Puoi utilizzare queste opzioni per specificare in modo esplicito quale vista deve essere salvata nei formati PDF, HTML o Immagine. Se questa proprietà è impostata,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) proprietà viene ignorata quando il progetto viene salvato. La vista dovrebbe provenire da una delle seguenti schermate (([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando viene chiamato il metodo set e viene fornita un'istanza della classe View con un valore non supportato della proprietà Screen. |

### Guarda anche

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* spazio dei nomi [Aspose.Tasks.Saving](../../saveoptions/)
* assemblea [Aspose.Tasks](../../../)


