---
title: "Κλάση HeaderFooterInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo κλάση. Αντιπροσωπεύει το οπτικό περιεχόμενο του κεφαλίδας/υποσέλιδου ή του υπομνήματος που χρησιμοποιείται για την εκτύπωση και απόδοση των προβολών."
type: docs
weight: 3130
url: /el/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Αναπαριστά το οπτικό περιεχόμενο της κεφαλίδας, του υποσέλιδου ή του υπομνήματος που χρησιμοποιείται για την εκτύπωση \\ απόδοση των προβολών.

```csharp
public class HeaderFooterInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `HeaderFooterInfo`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Λαμβάνει ή ορίζει την κεντραρισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της κεντρικής εικόνας. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Λαμβάνει ή ορίζει το κεντραρισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Λαμβάνει ή ορίζει την αριστερά ευθυγραμμισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της αριστερής εικόνας. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Λαμβάνει ή ορίζει το αριστερά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Λαμβάνει ή ορίζει την δεξιά ευθυγραμμισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της δεξιάς εικόνας. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Λαμβάνει ή ορίζει το δεξιά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε τις πληροφορίες κεφαλίδας/υποσέλιδου της σελίδας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


