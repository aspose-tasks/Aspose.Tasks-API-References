---
title: "Classe AvailabilityPeriodCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.AvailabilityPeriodCollection. Représente une collection qui contient des objets AvailabilityPeriod"
type: docs
weight: 90
url: /fr/net/aspose.tasks/availabilityperiodcollection/
---
## AvailabilityPeriodCollection class

Représente une collection qui contient des objets [`AvailabilityPeriod`](../availabilityperiod/).

```csharp
public class AvailabilityPeriodCollection : IList<AvailabilityPeriod>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/availabilityperiodcollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/availabilityperiodcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks/availabilityperiodcollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |
| [ParentResource](../../aspose.tasks/availabilityperiodcollection/parentresource/) { get; } | Obtient le parent [`Resource`](../resource/) pour cet objet. Objet parent [`Resource`](../resource/) pour cette collection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/availabilityperiodcollection/add/)(AvailabilityPeriod) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/availabilityperiodcollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/availabilityperiodcollection/contains/)(AvailabilityPeriod) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/availabilityperiodcollection/copyto/)(AvailabilityPeriod[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/availabilityperiodcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/availabilityperiodcollection/indexof/)(AvailabilityPeriod) | Détermine l'index de l'élément spécifié dans cette collection. |
| [Insert](../../aspose.tasks/availabilityperiodcollection/insert/)(int, AvailabilityPeriod) | Insère l'élément spécifié à l'index spécifié. |
| [Remove](../../aspose.tasks/availabilityperiodcollection/remove/)(AvailabilityPeriod) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [RemoveAt](../../aspose.tasks/availabilityperiodcollection/removeat/)(int) | Supprime un élément à l'index spécifié. |

## Exemples

Montre comment travailler avec la collection de périodes de disponibilité d'une ressource.

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // Ajoutez des périodes de disponibilité (années 2012 et 2014) à la nouvelle ressource
    IEnumerable<AvailabilityPeriod> periods = this.GetPeriods();
    foreach (var period in periods)
    {
        if (!resource.AvailabilityPeriods.IsReadOnly)
        {
            resource.AvailabilityPeriods.Add(period);
        }
    }

    var period2013 = new AvailabilityPeriod { AvailableFrom = new DateTime(2013, 1, 1), AvailableTo = new DateTime(2013, 12, 12), AvailableUnits = 0.81 };

    if (!resource.AvailabilityPeriods.Contains(period2013))
    {
        resource.AvailabilityPeriods.Insert(1, period2013);
    }

    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }

    var periodsToCopy = new AvailabilityPeriod[resource.AvailabilityPeriods.Count];
    resource.AvailabilityPeriods.CopyTo(periodsToCopy, 0);

    var otherResource = project.Resources.GetById(2);
    otherResource.AvailabilityPeriods.Clear();
    foreach (var period in periodsToCopy)
    {
        otherResource.AvailabilityPeriods.Add(period);
    }

    var period2015 = new AvailabilityPeriod { AvailableFrom = new DateTime(2015, 1, 1), AvailableTo = new DateTime(2015, 12, 12), AvailableUnits = 0.50 };

    var period2016 = new AvailabilityPeriod { AvailableFrom = new DateTime(2016, 1, 1), AvailableTo = new DateTime(2016, 12, 12), AvailableUnits = 0.53 };

    if (otherResource.AvailabilityPeriods.IndexOf(period2015) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2015);
    }

    if (otherResource.AvailabilityPeriods.IndexOf(period2016) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2016);
    }

    // mettre à jour les unités disponibles pour la période de l'année 2014
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // supprimer la période de 2013
    otherResource.AvailabilityPeriods.Remove(period2013);

    // supprimer la période de 2011
    otherResource.AvailabilityPeriods.RemoveAt(0);

    Console.WriteLine("Print resource availability periods of the resource: " + otherResource.Get(Rsc.Name));
    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>();
    var period = new AvailabilityPeriod { AvailableFrom = new DateTime(2012, 1, 1), AvailableTo = new DateTime(2012, 12, 12), AvailableUnits = 0.99 };
    periods.Add(period);

    var period2 = new AvailabilityPeriod { AvailableFrom = new DateTime(2014, 1, 1), AvailableTo = new DateTime(2014, 12, 12), AvailableUnits = 0.94 };
    periods.Add(period2);
    return periods;
}
```

### Voir aussi

* class [AvailabilityPeriod](../availabilityperiod/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


