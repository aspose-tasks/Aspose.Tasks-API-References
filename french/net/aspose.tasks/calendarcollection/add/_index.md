---
title: "CalendarCollection.Add"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Ajoute un nouveau calendrier de base à cet objet CalendarCollection et retourne le calendrier ajouté."
type: docs
weight: 20
url: /fr/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Ajoute un nouveau calendrier de base à cet objet CalendarCollection et renvoie le calendrier ajouté.

```csharp
public Calendar Add(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | Chaîne | Nom du calendrier. |

### Valeur de retour

Objet [`Calendar`](../../calendar/) ajouté.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancé lorsque le nom du calendrier est nul. |

## Exemples

Montre comment créer un calendrier standard.

```csharp
var project = new Project();

// Définissez un calendrier et rendez-le standard
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Ajoute un nouveau calendrier avec le calendrier de base spécifié à cet objet CalendarCollection et renvoie le calendrier ajouté.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | Chaîne | Nom spécifié. |
| baseCalendar | Calendar | Calendrier de base spécifié. |

### Valeur de retour

Objet [`Calendar`](../../calendar/) ajouté.

## Exemples

Montre comment ajouter de nouveaux calendriers.

```csharp
var project = new Project();

// De nouveaux calendriers peuvent être ajoutés à la collection de calendriers d'un projet en utilisant les surcharges de la méthode Add de la collection.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


