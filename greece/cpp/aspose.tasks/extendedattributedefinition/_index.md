---
title: "Aspose::Tasks::ExtendedAttributeDefinition κλάση"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks για C++"
description: "Αντιπροσωπεύει έναν ορισμό επεκταμένου χαρακτηριστικού που σχετίζεται με ένα έργο."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Αντιπροσωπεύει έναν ορισμό επεκταμένου χαρακτηριστικού που σχετίζεται με ένα έργο.

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Προσθέτει μια τιμή στη εσωτερική λίστα αναζήτησης. Αυτή είναι η προτιμώμενη μέθοδος για χειρισμούς με το ValueList . |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το ID πεδίου που ισούται με την τιμή του ID πεδίου αυτού του αντικειμένου. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο. |
| [Equals](./equals/) | Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο. |
| [get_Alias](./get_alias/) | Λαμβάνει το ψευδώνυμο ενός προσαρμοσμένου πεδίου. |
| [get_AppendNewValues](./get_appendnewvalues/) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι νέες τιμές που προστίθενται σε ένα έργο προστίθενται αυτόματα στη λίστα. |
| [get_AutoRollDown](./get_autorolldown/) | Λαμβάνει μια τιμή που υποδεικνύει εάν είναι ενεργοποιημένη η αυτόματη μεταφορά σε αναθέσεις. |
| [get_CalculationType](./get_calculationtype/) | Λαμβάνει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού. |
| [get_CfType](./get_cftype/) | Λαμβάνει τον τύπο ενός προσαρμοσμένου πεδίου. |
| [get_Default](./get_default/) | Λαμβάνει την προεπιλεγμένη τιμή στη λίστα. |
| [get_DefaultGuid](./get_defaultguid/) | Λαμβάνει το Guid της προεπιλεγμένης καταχώρησης του πίνακα αναζήτησης. |
| [get_ElementType](./get_elementtype/) | Λαμβάνει το εκτεταμένο χαρακτηριστικό που συσχετίζεται με μια εργασία, έναν πόρο ή μια ανάθεση. |
| [get_FieldId](./get_fieldid/) | Λαμβάνει το αναγνωριστικό έργου ενός προσαρμοσμένου πεδίου. Χρησιμοποιήστε την αναπαράσταση συμβολοσειράς μιας σταθεράς από την κλάση Aspose::Tasks::ExtendedAttributeTask για να ορίσετε την ιδιότητα FieldId. |
| [get_FieldName](./get_fieldname/) | Λαμβάνει το όνομα ενός προσαρμοσμένου πεδίου. |
| [get_Formula](./get_formula/) | Λαμβάνει τον τύπο που χρησιμοποιεί το Microsoft Project για τη συμπλήρωση ενός προσαρμοσμένου πεδίου εργασίας. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Λαμβάνει πληροφορίες γραφικών δεικτών που σχετίζονται με το εκτεταμένο χαρακτηριστικό. Εφαρμόσιμο στη μορφή MPP. |
| [get_Guid](./get_guid/) | Λαμβάνει το Guid ενός προσαρμοσμένου πεδίου. |
| [get_LookupUid](./get_lookupuid/) | Λαμβάνει ένα Guid του πίνακα αναζήτησης που σχετίζεται με ένα προσαρμοσμένο πεδίο. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Λαμβάνει τον μέγιστο αριθμό τιμών που μπορείτε να ορίσετε σε μια λίστα επιλογής. |
| [get_ParentProject](./get_parentproject/) | Λαμβάνει το γονικό έργο για την παρουσία ExtendedAttributeDefinition. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Λαμβάνει τη φωνητική προφορά του ψευδώνυμου ενός προσαρμοσμένου πεδίου. |
| [get_RestrictValues](./get_restrictvalues/) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι τιμές του προσαρμοσμένου πεδίου περιορίζονται στις τιμές του ValueList. |
| [get_RollupType](./get_rolluptype/) | Λαμβάνει τον τρόπο υπολογισμού των συγκεντρώσεων. |
| [get_SecondaryGuid](./get_secondaryguid/) | Λαμβάνει το δευτερεύον guid του εκτεταμένου χαρακτηριστικού. |
| [get_SecondaryPid](./get_secondarypid/) | Λαμβάνει το δευτερεύον PID ενός προσαρμοσμένου πεδίου. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Λαμβάνει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης. |
| [get_UserDef](./get_userdef/) | Λαμβάνει μια τιμή που υποδεικνύει εάν ένα προσαρμοσμένο πεδίο ορίζεται από τον χρήστη. |
| [get_ValueList](./get_valuelist/) | Λαμβάνει το List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Λαμβάνει τον τρόπο ταξινόμησης των λιστών τιμών. Οι τιμές είναι: 0=Φθίνουσα, 1=Αύξουσα. |
| [GetHashCode](./gethashcode/) | Επιστρέφει έναν κώδικα κατακερματισμού για την παρουσία της κλάσης ExtendedAttributeDefinition. |
| [RemoveLookupValue](./removelookupvalue/) | Αφαιρεί μια τιμή από την εσωτερική λίστα αναζήτησης. Αυτός είναι ο προτιμώμενος τρόπος για χειρισμούς με το ValueList. |
| [set_Alias](./set_alias/) | Ορίζει το ψευδώνυμο ενός προσαρμοσμένου πεδίου. |
| [set_AppendNewValues](./set_appendnewvalues/) | Ορίζει μια τιμή που υποδεικνύει εάν οι νέες τιμές που προστίθενται σε ένα έργο προστίθενται αυτόματα στη λίστα. |
| [set_AutoRollDown](./set_autorolldown/) | Ορίζει μια τιμή που υποδεικνύει εάν είναι ενεργοποιημένο το αυτόματο κατέβασμα σε εκχωρήσεις. |
| [set_CalculationType](./set_calculationtype/) | Ορίζει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού. |
| [set_Default](./set_default/) | Ορίζει την προεπιλεγμένη τιμή στη λίστα. |
| [set_DefaultGuid](./set_defaultguid/) | Ορίζει το Guid της προεπιλεγμένης καταχώρησης πίνακα αναζήτησης. |
| [set_ElementType](./set_elementtype/) | Ορίζει ότι το εκτεταμένο χαρακτηριστικό συνδέεται με μια εργασία, έναν πόρο ή μια εκχώρηση. |
| [set_FieldId](./set_fieldid/) | Ορίζει που αντιστοιχεί στο αναγνωριστικό έργου ενός προσαρμοσμένου πεδίου. Χρησιμοποιήστε την αναπαράσταση συμβολοσειράς μιας σταθεράς από την κλάση **Aspose::Tasks::ExtendedAttributeTask** για να καθορίσετε την ιδιότητα **FieldId**. |
| [set_Formula](./set_formula/) | Ορίζει τον τύπο που χρησιμοποιεί το Microsoft Project για να γεμίσει ένα προσαρμοσμένο πεδίο εργασίας. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Ορίζει πληροφορίες γραφικών δεικτών που σχετίζονται με το εκτεταμένο χαρακτηριστικό. Εφαρμόσιμο στη μορφή MPP. |
| [set_Guid](./set_guid/) | Ορίζει το Guid ενός προσαρμοσμένου πεδίου. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Ορίζει τον μέγιστο αριθμό τιμών που μπορείτε να ορίσετε σε μια λίστα επιλογών. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Ορίζει τη φωνητική προφορά του ψευδώνυμου ενός προσαρμοσμένου πεδίου. |
| [set_RestrictValues](./set_restrictvalues/) | Ορίζει μια τιμή που υποδεικνύει εάν οι τιμές του προσαρμοσμένου πεδίου περιορίζονται στις τιμές της **ValueList**. |
| [set_RollupType](./set_rolluptype/) | Ορίζει τον τρόπο με τον οποίο υπολογίζονται οι συγκεντρωτικές τιμές. |
| [set_SecondaryGuid](./set_secondaryguid/) | Ορίζει το δευτερεύον guid του εκτεταμένου χαρακτηριστικού. |
| [set_SecondaryPid](./set_secondarypid/) | Ορίζει το δευτερεύον PID ενός προσαρμοσμένου πεδίου. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Ορίζει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού για γραμμές σύνοψης. |
| [set_UserDef](./set_userdef/) | Ορίζει μια τιμή που υποδεικνύει εάν ένα προσαρμοσμένο πεδίο ορίζεται από τον χρήστη. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Ορίζει τον τρόπο ταξινόμησης των λιστών τιμών. Οι τιμές είναι: 0=Φθίνουσα, 1=Αύξουσα. |

