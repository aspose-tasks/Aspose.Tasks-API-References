---
title: "License.SetLicense"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος License. Παρέχει άδεια στο στοιχείο."
type: docs
weight: 20
url: /el/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Αδειοδοτεί το στοιχείο.

```csharp
public void SetLicense(string licenseName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| licenseName | String | Μπορεί να είναι πλήρες ή σύντομο όνομα αρχείου ή όνομα ενσωματωμένου πόρου. Χρησιμοποιήστε μια κενή συμβολοσειρά για να μεταβείτε σε λειτουργία αξιολόγησης. |

## Παρατηρήσεις

Προσπαθεί να βρει την άδεια στις ακόλουθες τοποθεσίες:

1. Ρητή διαδρομή.

2. Ο φάκελος που περιέχει τη συναρμολόγηση του στοιχείου Aspose.

3. Ο φάκελος που περιέχει τη συναρμολόγηση κλήσης του πελάτη.

4. Ο φάκελος που περιέχει τη συναρμολόγηση εισόδου (εκκίνησης).

5. Ένας ενσωματωμένος πόρος στη συναρμολόγηση κλήσης του πελάτη.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Ρητή διαδρομή.

2. Ένας ενσωματωμένος πόρος στη συναρμολόγηση κλήσης του πελάτη.

2. Ο φάκελος που περιέχει το αρχείο JAR του στοιχείου Aspose.

3. Ο φάκελος που περιέχει το αρχείο JAR κλήσης του πελάτη.

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να βρεθεί ένα αρχείο άδειας με όνομα MyLicense.lic στο φάκελο που περιέχει το στοιχείο, στο φάκελο που περιέχει το καλούν σύνολο, στο φάκελο του κύριου συνόλου και στη συνέχεια στους ενσωματωμένους πόρους του καλούντος συνόλου.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

το αρχείο component jar:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Δείχνει πώς να εφαρμόσετε μια άδεια του Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Δείτε επίσης

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

Αδειοδοτεί το στοιχείο.

```csharp
public void SetLicense(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Μία ροή που περιέχει την άδεια. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτή τη μέθοδο για να φορτώσετε μια άδεια από μια ροή.

## Παραδείγματα

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Δείχνει πώς να εφαρμόσετε μια άδεια του Aspose.Tasks που διαβάζεται από &lt;see cref=\"System.IO.FileStream\" /&gt;.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### Δείτε επίσης

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


