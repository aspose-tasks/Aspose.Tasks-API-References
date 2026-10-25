---
title: "Κλάση Rate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Rate. Αντιπροσωπεύει έναν ορισμό χρονικής περιόδου και τιμών που ισχύουν για έναν πόρο κατά τη διάρκεια αυτής της περιόδου"
type: docs
weight: 1610
url: /el/net/aspose.tasks/rate/
---
## Rate class

Αντιπροσωπεύει έναν ορισμό χρονικής περιόδου και τιμών που ισχύουν για έναν πόρο κατά τη διάρκεια αυτής της περιόδου.

```csharp
public class Rate
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Λαμβάνει ή ορίζει το κόστος ανά χρήση ενός πόρου. Αυτή η τιμή λαμβάνεται από την τρέχουσα ημερομηνία εάν υπάρχει πίνακας τιμών για έναν πόρο. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Λαμβάνει ή ορίζει το ωριαίο ποσοστό υπερωρίας για έναν πόρο. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Λαμβάνει ή ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ποσοστού υπερωρίας. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία έναρξης ισχύος μιας τιμής. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Λαμβάνει ή ορίζει την τελευταία ημερομηνία ισχύος μιας τιμής. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό ενός πίνακα τιμών για έναν πόρο. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Λαμβάνει ή ορίζει το τυπικό ωριαίο ποσοστό για έναν πόρο. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Λαμβάνει ή ορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ποσοστού. |

## Παραδείγματα

Δείχνει πώς να εργάζεστε με τιμές πόρων.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


