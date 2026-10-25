---
title: "Rsc.BookingType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le type de réservation d'une ressource"
type: docs
weight: 160
url: /fr/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Le type de réservation d'une ressource.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


