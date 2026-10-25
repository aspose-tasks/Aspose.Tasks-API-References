---
title: "Événement"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Un événement."
type: docs
weight: 374
url: /fr/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Un événement.

`TArgs`: arguments de l'événement.

TArgs :
## Méthodes

| Méthode | Description |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Cette méthode est invoquée lorsque l'événement est émis. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Cette méthode est invoquée lorsque l'événement est émis.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | un objet qui initie cet événement. |
| args | TArgs | arguments personnalisés. |

