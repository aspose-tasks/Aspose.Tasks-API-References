---
title: "Rsc"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει τις υποστηριζόμενες ιδιότητες του αντικειμένου Resource."
type: docs
weight: 271
url: /el/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

Αντιπροσωπεύει τις υποστηριζόμενες ιδιότητες του αντικειμένου `Resource`.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | Καθορίζει πώς και πότε τα τυπικά και υπερωριακά κόστη του πόρου πρέπει να χρεωθούν ή να συσσωρευτούν στο κόστος μιας εργασίας. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | Το Guid του Active Directory για έναν πόρο. |
| [ACTUAL_COST](#ACTUAL-COST) | Κόστη που προκύπτουν από εργασία που έχει ήδη εκτελεστεί από πόρους στις εργασίες τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με την εργασία. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Κόστη που προέκυψαν για υπερωριακή εργασία που ήδη εκτελέστηκε σε εργασίες από τους ανατεθειμένους πόρους. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | Το πραγματικό ποσό της υπερωριακής εργασίας που ήδη εκτελέστηκε από τον πόρο που έχει ανατεθεί σε εργασίες. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική υπερωριακή εργασία. |
| [ACTUAL_WORK](#ACTUAL-WORK) | Το ποσό εργασίας που έχει ήδη ολοκληρωθεί από τον πόρο που έχει ανατεθεί σε εργασίες. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική εργασία. |
| [ACWP](#ACWP) | Το πραγματικό κόστος μιας εργασίας που εκτελέστηκε από έναν πόρο για το έργο μέχρι σήμερα. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | Το όνομα του ιδιοκτήτη της ανάθεσης. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | Το GUID του ιδιοκτήτη της ανάθεσης. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | Η ημερομηνία έναρξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο. |
| [AVAILABLE_TO](#AVAILABLE-TO) | Η ημερομηνία λήξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο. |
| [BCWP](#BCWP) | Το προϋπολογισμένο κόστος μιας εργασίας που εκτελέστηκε από έναν πόρο για το έργο μέχρι σήμερα. |
| [BCWS](#BCWS) | Το προϋπολογιστικό κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο. |
| [BOOKING_TYPE](#BOOKING-TYPE) | Ο τύπος κράτησης ενός πόρου. |
| [BUDGET_COST](#BUDGET-COST) | Προϋπολογιστικά κόστη για πόρους προϋπολογιστικού κόστους. |
| [BUDGET_WORK](#BUDGET-WORK) | προϋπολογιστική εργασία για προϋπολογιστική εργασία και υλικούς πόρους. |
| [CALENDAR](#CALENDAR) | Το ημερολόγιο ενός πόρου. |
| [CAN_LEVEL](#CAN-LEVEL) | Καθορίζει εάν μπορεί να γίνει εξισορρόπηση πόρων σε έναν πόρο. |
| [CODE](#CODE) | Ο κώδικας ή άλλες πληροφορίες σχετικά με έναν πόρο. |
| [COST](#COST) | Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για έναν πόρο, βασισμένο στα κόστη που έχουν ήδη προκύψει για εργασία που εκτελέστηκε από πόρους που έχουν ανατεθεί στις εργασίες, επιπλέον των κόστους που έχουν προγραμματιστεί για την υπόλοιπη εργασία. |
| [COST_CENTER](#COST-CENTER) | Δείχνει σε ποιο κέντρο κόστους πρέπει να χρεωθούν τα κόστη που συσσωρεύονται από τον πόρο. |
| [COST_PER_USE](#COST-PER-USE) | Το κόστος που συσσωρεύεται κάθε φορά που χρησιμοποιείται ένας πόρος. |
| [COST_VARIANCE](#COST-VARIANCE) | Η διαφορά μεταξύ του βασικού κόστους και του συνολικού κόστους για έναν πόρο. |
| [CREATED](#CREATED) | Η ημερομηνία και ώρα που προστέθηκε ένας πόρος στο έργο. |
| [CV](#CV) | Η διακύμανση κόστους της κερδισμένης αξίας, μέχρι την ημερομηνία κατάστασης του έργου. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | Η διεύθυνση email ενός πόρου. |
| [FINISH](#FINISH) | Η ημερομηνία κατά την οποία ένας πόρος προγραμματίζεται να ολοκληρώσει την εργασία σε όλες τις εκχωρημένες εργασίες. |
| [GROUP](#GROUP) | Η ομάδα στην οποία ανήκει ένας πόρος. |
| [GUID](#GUID) | Περιέχει τον παραγόμενο μοναδικό κωδικό ταυτοποίησης για τον πόρο. |
| [HYPERLINK](#HYPERLINK) | Ο τίτλος ή το εξηγητικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | Η διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | Η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία. |
| [ID](#ID) | Το αναγνωριστικό θέσης ενός πόρου στη λίστα των πόρων. |
| [INACTIVE](#INACTIVE) | Καθορίζει εάν ένας πόρος καταστήθηκε ανενεργός από χρήστη με διαχειριστικά δικαιώματα. |
| [INITIALS](#INITIALS) | Τα αρχικά ενός πόρου. |
| [IS_BUDGET](#IS-BUDGET) | Καθορίζει εάν ένας πόρος εργασίας, υλικού ή κόστους είναι πόρος προϋπολογισμού. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | Καθορίζει εάν ένας πόρος είναι πόρος κόστους. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | Δείχνει εάν ένας πόρος προέρχεται από την εταιρική δεξαμενή πόρων (true) ή από την τοπική δεξαμενή πόρων (false). |
| [IS_GENERIC](#IS-GENERIC) | Καθορίζει εάν ένας πόρος είναι γενικός ή όχι. |
| [IS_NULL](#IS-NULL) | Καθορίζει εάν ένας πόρος είναι null. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | Δείχνει εάν ο τρέχων πόρος είναι πόρος ομάδας. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | Η μονάδα μέτρησης για τον πόρο υλικού. |
| [MAX_UNITS](#MAX-UNITS) | Ο μέγιστος αριθμός μονάδων που αντιπροσωπεύει τη μέγιστη χωρητικότητα για την οποία ένας πόρος είναι διαθέσιμος να ολοκληρώσει οποιεσδήποτε εργασίες κατά την τρέχουσα χρονική περίοδο. |
| [NAME](#NAME) | Το όνομα ενός πόρου. |
| [NOTES_RTF](#NOTES-RTF) | Οι σημειώσεις κειμένου σε μορφή RTF. |
| [NOTES_TEXT](#NOTES-TEXT) | Το απλό κείμενο των σημειώσεων που εξάγεται από δεδομένα RTF. |
| [OVERALLOCATED](#OVERALLOCATED) | Δείχνει εάν ένας πόρος έχει εκχωρηθεί σε περισσότερη εργασία σε μια συγκεκριμένη εργασία ή σε όλες τις εργασίες από ό,τι μπορεί να ολοκληρωθεί εντός της κανονικής εργασιακής χωρητικότητας. |
| [OVERTIME_COST](#OVERTIME-COST) | Το συνολικό κόστος υπερωριών για έναν πόρο σε όλες τις εκχωρημένες εργασίες. |
| [OVERTIME_RATE](#OVERTIME-RATE) | Ο ρυθμός αμοιβής για την υπερωριακή εργασία που εκτελείται από έναν πόρο. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του υπερωριακού ρυθμού. |
| [OVERTIME_WORK](#OVERTIME-WORK) | Το ποσό των υπερωριών που προγραμματίζεται να εκτελεστεί από έναν πόρο σε μια εργασία και χρεώνεται με τους υπερωριακούς ρυθμούς των εμπλεκόμενων πόρων. |
| [PEAK_UNITS](#PEAK-UNITS) | Η μέγιστη μονάδα ανάθεσης για έναν πόρο σε οποιαδήποτε χρονική στιγμή για όλες τις εργασίες στις οποίες έχει ανατεθεί ο πόρος. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | Το ποσοστό του ολοκληρωμένου έργου σε όλες τις εργασίες. |
| [PHONETICS](#PHONETICS) | Η φωνητική γραφή του ονόματος του πόρου. |
| [REGULAR_WORK](#REGULAR-WORK) | Το συνολικό ποσό μη υπερωριακής εργασίας που έχει προγραμματιστεί να εκτελεστεί από τον πόρο. |
| [REMAINING_COST](#REMAINING-COST) | Το υπόλοιπο προγραμματισμένο έξοδο που θα προκύψει στην ολοκλήρωση της υπόλοιπης προγραμματισμένης εργασίας. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | Το υπόλοιπο προγραμματισμένο έξοδο υπερωριών για έναν πόρο. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | Το ποσό των υπόλοιπων προγραμματισμένων υπερωριών. |
| [REMAINING_WORK](#REMAINING-WORK) | Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή συνόλου εργασιών. |
| [STANDARD_RATE](#STANDARD-RATE) | Ο ρυθμός αμοιβής για κανονική, μη υπερωριακή εργασία που εκτελείται από έναν πόρο. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ρυθμού. |
| [START](#START) | Η ημερομηνία κατά την οποία ένας ανατεθειμένος πόρος έχει προγραμματιστεί να αρχίσει να εργάζεται σε μια εργασία. |
| [SV](#SV) | Η διακύμανση του χρονοδιαγράμματος αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. |
| [TYPE](#TYPE) | Ο τύπος ενός πόρου. |
| [UID](#UID) | Το μοναδικό αναγνωριστικό ενός πόρου. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | Ο λογαριασμός NT που συνδέεται με έναν πόρο. |
| [WORK](#WORK) | Το συνολικό ποσό χρόνου που έχει προγραμματιστεί για έναν πόρο σε μια εργασία. |
| [WORKGROUP](#WORKGROUP) | Ο τύπος μιας ομάδας εργασίας στην οποία ανήκει ένας πόρος. |
| [WORK_VARIANCE](#WORK-VARIANCE) | Η διαφορά μεταξύ της βασικής εργασίας ενός πόρου και της τρέχουσας προγραμματισμένης εργασίας. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


Καθορίζει πώς και πότε τα τυπικά και υπερωριακά κόστη του πόρου πρέπει να χρεωθούν ή να συσσωρευτούν στο κόστος μιας εργασίας.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


Το Guid του Active Directory για έναν πόρο.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Κόστη που προκύπτουν από εργασία που έχει ήδη εκτελεστεί από πόρους στις εργασίες τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με την εργασία.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Κόστη που προέκυψαν για υπερωριακή εργασία που ήδη εκτελέστηκε σε εργασίες από τους ανατεθειμένους πόρους.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


Το πραγματικό ποσό της υπερωριακής εργασίας που ήδη εκτελέστηκε από τον πόρο που έχει ανατεθεί σε εργασίες.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική υπερωριακή εργασία.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


Το ποσό εργασίας που έχει ήδη ολοκληρωθεί από τον πόρο που έχει ανατεθεί σε εργασίες.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική εργασία.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


Το πραγματικό κόστος μιας εργασίας που εκτελέστηκε από έναν πόρο για το έργο μέχρι σήμερα.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


Το όνομα του ιδιοκτήτη της ανάθεσης.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


Το GUID του ιδιοκτήτη της ανάθεσης.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


Η ημερομηνία έναρξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


Η ημερομηνία λήξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


Το προϋπολογισμένο κόστος μιας εργασίας που εκτελέστηκε από έναν πόρο για το έργο μέχρι σήμερα.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


Το προϋπολογιστικό κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


Ο τύπος κράτησης ενός πόρου.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Κόστη προϋπολογισμού για πόρους κόστους προϋπολογισμού. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία σύνοψης του έργου.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


Εργασία προϋπολογισμού για πόρους εργασίας προϋπολογισμού και υλικών. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία σύνοψης του έργου.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


Το ημερολόγιο ενός πόρου.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


Καθορίζει εάν μπορεί να γίνει εξισορρόπηση πόρων σε έναν πόρο.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


Ο κώδικας ή άλλες πληροφορίες σχετικά με έναν πόρο.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για έναν πόρο, βασισμένο στα κόστη που έχουν ήδη προκύψει για εργασία που εκτελέστηκε από πόρους που έχουν ανατεθεί στις εργασίες, επιπλέον των κόστους που έχουν προγραμματιστεί για την υπόλοιπη εργασία.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


Δείχνει σε ποιο κέντρο κόστους πρέπει να χρεωθούν τα κόστη που συσσωρεύονται από τον πόρο.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


Το κόστος που συσσωρεύεται κάθε φορά που χρησιμοποιείται ένας πόρος.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


Η διαφορά μεταξύ του βασικού κόστους και του συνολικού κόστους για έναν πόρο.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


Η ημερομηνία και ώρα που προστέθηκε ένας πόρος στο έργο.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


Η διακύμανση κόστους αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Το CV είναι η διαφορά μεταξύ του BCWP (προϋπολογισμένο κόστος εκτελεσθείσας εργασίας) και του ACWP (πραγματικό κόστος εκτελεσθείσας εργασίας) της εργασίας.

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


Η διεύθυνση email ενός πόρου.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


Η ημερομηνία κατά την οποία ένας πόρος προγραμματίζεται να ολοκληρώσει την εργασία σε όλες τις εκχωρημένες εργασίες.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


Η ομάδα στην οποία ανήκει ένας πόρος.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


Περιέχει τον παραγόμενο μοναδικό κωδικό ταυτοποίησης για τον πόρο.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


Ο τίτλος ή το εξηγητικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


Η διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


Η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με μια εργασία.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


Το αναγνωριστικό θέσης ενός πόρου στη λίστα των πόρων.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


Καθορίζει εάν ένας πόρος καταστήθηκε ανενεργός από χρήστη με διαχειριστικά δικαιώματα.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


Τα αρχικά ενός πόρου.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


Καθορίζει εάν ένας πόρος εργασίας, υλικού ή κόστους είναι πόρος προϋπολογισμού.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


Καθορίζει εάν ένας πόρος είναι πόρος κόστους.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


Δείχνει εάν ένας πόρος προέρχεται από την εταιρική δεξαμενή πόρων (true) ή από την τοπική δεξαμενή πόρων (false).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


Καθορίζει εάν ένας πόρος είναι γενικός ή όχι.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Καθορίζει εάν ένας πόρος είναι null.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


Δείχνει εάν ο τρέχων πόρος είναι πόρος ομάδας.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


Η μονάδα μέτρησης για τον πόρο υλικού.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


Ο μέγιστος αριθμός μονάδων που αντιπροσωπεύει τη μέγιστη χωρητικότητα για την οποία ένας πόρος είναι διαθέσιμος να ολοκληρώσει οποιεσδήποτε εργασίες κατά την τρέχουσα χρονική περίοδο.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


Το όνομα ενός πόρου.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


Οι σημειώσεις κειμένου σε μορφή RTF.

--------------------

Υποστηρίζεται μόνο για μορφές MPP.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


Το απλό κείμενο των σημειώσεων που εξάγεται από δεδομένα RTF.

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


Δείχνει εάν ένας πόρος έχει εκχωρηθεί σε περισσότερη εργασία σε μια συγκεκριμένη εργασία ή σε όλες τις εργασίες από ό,τι μπορεί να ολοκληρωθεί εντός της κανονικής εργασιακής χωρητικότητας.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


Το συνολικό κόστος υπερωριών για έναν πόρο σε όλες τις εκχωρημένες εργασίες.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


Ο ρυθμός αμοιβής για την υπερωριακή εργασία που εκτελείται από έναν πόρο.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του υπερωριακού ρυθμού.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


Το ποσό των υπερωριών που προγραμματίζεται να εκτελεστεί από έναν πόρο σε μια εργασία και χρεώνεται με τους υπερωριακούς ρυθμούς των εμπλεκόμενων πόρων.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


Η μέγιστη μονάδα ανάθεσης για έναν πόρο σε οποιαδήποτε χρονική στιγμή για όλες τις εργασίες στις οποίες έχει ανατεθεί ο πόρος.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


Το ποσοστό του ολοκληρωμένου έργου σε όλες τις εργασίες.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


Η φωνητική γραφή του ονόματος του πόρου. Για χρήση μόνο με Ιαπωνικά.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


Το συνολικό ποσό μη υπερωριακής εργασίας που έχει προγραμματιστεί να εκτελεστεί από τον πόρο.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


Το υπόλοιπο προγραμματισμένο έξοδο που θα προκύψει στην ολοκλήρωση της υπόλοιπης προγραμματισμένης εργασίας.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


Το υπόλοιπο προγραμματισμένο έξοδο υπερωριών για έναν πόρο.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


Το ποσό των υπόλοιπων προγραμματισμένων υπερωριών.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή συνόλου εργασιών.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


Ο ρυθμός αμοιβής για κανονική, μη υπερωριακή εργασία που εκτελείται από έναν πόρο.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ρυθμού.

### START {#START}
```
public static final Key<Date,Byte> START
```


Η ημερομηνία κατά την οποία ένας ανατεθειμένος πόρος έχει προγραμματιστεί να αρχίσει να εργάζεται σε μια εργασία.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


Η διακύμανση του χρονοδιαγράμματος αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Το SV είναι η διαφορά μεταξύ του προϋπολογισμένου κόστους εκτελεσθείσας εργασίας (BCWP) και του προϋπολογισμένου κόστους προγραμματισμένης εργασίας (BCWS).

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


Ο τύπος ενός πόρου.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


Το μοναδικό αναγνωριστικό ενός πόρου.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


Ο λογαριασμός NT που συνδέεται με έναν πόρο.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


Το συνολικό ποσό χρόνου που έχει προγραμματιστεί για έναν πόρο σε μια εργασία.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


Ο τύπος μιας ομάδας εργασίας στην οποία ανήκει ένας πόρος.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


Η διαφορά μεταξύ της βασικής εργασίας ενός πόρου και της τρέχουσας προγραμματισμένης εργασίας.

