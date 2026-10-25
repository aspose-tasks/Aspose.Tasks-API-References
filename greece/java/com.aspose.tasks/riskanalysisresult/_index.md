---
title: "RiskAnalysisResult"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει ένα αποτέλεσμα ανάλυσης κινδύνου."
type: docs
weight: 262
url: /el/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Αντιπροσωπεύει ένα αποτέλεσμα ανάλυσης κινδύνου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Επιστρέφει ένα στιγμιότυπο της [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) για τον καθορισμένο τύπο κινδύνου. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη ροή σε μορφή PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη καθορισμένη διαδρομή αρχείου σε μορφή PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Επιστρέφει ένα στιγμιότυπο της [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) για τον καθορισμένο τύπο κινδύνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| itemType | int | ο καθορισμένος τύπος κινδύνου· μπορεί να είναι μία από τις τιμές της απαρίθμησης [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη ροή σε μορφή PDF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | Η ροή στην οποία θα αποθηκευτεί η αναφορά ανάλυσης κινδύνου. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη καθορισμένη διαδρομή αρχείου σε μορφή PDF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το καθορισμένο όνομα αρχείου. |

