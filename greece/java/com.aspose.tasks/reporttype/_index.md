---
title: "ReportType"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Τύπος του γραφικού αναφοράς των έργων."
type: docs
weight: 247
url: /el/java/com.aspose.tasks/reporttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ReportType extends System.Enum
```

Τύπος του γραφικού αναφοράς του έργου.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [BestPracticeAnalyzer](#BestPracticeAnalyzer) | Εμφανίζει εργασίες χωρίς πραγματική εργασία, μη εκχωρημένες εργασίες, εργασίες με διάρκεια μικρότερη από 8 ώρες και περιλήψεις που έχουν εκχωρηθεί στους πόρους. |
| [Burndown](#Burndown) | Περιλαμβάνει διαγράμματα κατανάλωσης εργασίας και διαγράμματα κατανάλωσης εργασιών. |
| [CashFlow](#CashFlow) | Εμφανίζει τα κόστη και τα συσσωρευμένα κόστη ανά τρίμηνο για όλες τις εργασίες υψηλότερου επιπέδου. |
| [CostOverruns](#CostOverruns) | Εμφανίζει τη διακύμανση κόστους ανά εργασία και πόρο. |
| [CostOverview](#CostOverview) | Εμφανίζει τις ημερομηνίες έναρξης και λήξης του έργου, το τρέχον προγραμματισμένο και εναπομείναν κόστος, το % ολοκλήρωσης και τις τιμές κόστους για εργασίες υψηλότερου επιπέδου. |
| [CriticalTasks](#CriticalTasks) | Εμφανίζει τις εργασίες του έργου που είναι κρίσιμες. |
| [LateTasks](#LateTasks) | Εμφανίζει τις εργασίες του έργου που είναι καθυστερημένες. |
| [Milestones](#Milestones) | Εμφανίζει ορόσημα που είναι καθυστερημένα, επερχόμενα και ολοκληρωμένα. |
| [OverallocatedResources](#OverallocatedResources) | Εμφανίζει τον αριθμό των εναπομείναντων ωρών εργασίας για υπερκατανεμημένους πόρους. |
| [ProjectOverview](#ProjectOverview) | Εμφανίζει την ημερομηνία έναρξης και λήξης του project\u2019s, το ποσοστό της διάρκειας που\u2019s ολοκληρώθηκε, το ποσοστό ολοκλήρωσης για εργασίες ανώτερου επιπέδου και τα επερχόμενα ορόσημα. |
| [ResourceCostOverview](#ResourceCostOverview) | Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν κόστος ανά πόρο. |
| [ResourceOverview](#ResourceOverview) | Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν έργο ανά πόρο. |
| [SlippingTasks](#SlippingTasks) | Εμφανίζει εργασίες που πρέπει να ολοκληρωθούν μετά τις ημερομηνίες λήξης της γραμμής βάσης (η γραμμή βάσης πρέπει να είναι setInternal). |
| [TaskCostOverview](#TaskCostOverview) | Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν κόστος όλων των εργασιών ανώτερου επιπέδου. |
| [UpcomingTask](#UpcomingTask) | Εμφανίζει εργασίες που λήγουν κατά τη διάρκεια της τρέχουσας εβδομάδας και εργασίες που ξεκινούν κατά τη διάρκεια της τρέχουσας εβδομάδας. |
| [WorkOverview](#WorkOverview) | Εμφανίζει τη γραμμή βάσης, το πραγματικό, το εναπομείναν έργο για κάθε εργασία ανώτερου επιπέδου και εργασία για πόρους εργασίας. |
### BestPracticeAnalyzer {#BestPracticeAnalyzer}
```
public static final int BestPracticeAnalyzer
```


Εμφανίζει εργασίες χωρίς πραγματική εργασία, μη εκχωρημένες εργασίες, εργασίες με διάρκεια μικρότερη από 8 ώρες και περιλήψεις που έχουν εκχωρηθεί στους πόρους.

### Burndown {#Burndown}
```
public static final int Burndown
```


Περιλαμβάνει διαγράμματα κατανάλωσης εργασίας και διαγράμματα κατανάλωσης εργασιών. Το διάγραμμα κατανάλωσης εργασίας δείχνει πόση εργασία έχουν ολοκληρώσει οι άνθρωποι, πόση είναι προγραμματισμένη να ολοκληρωθεί πριν από την ημερομηνία λήξης του έργου, και την εκτίμηση της γραμμής βάσης για το πόση εργασία θα ολοκληρωνόταν σε αυτό το σημείο του έργου. Το διάγραμμα κατανάλωσης εργασιών δείχνει τον αριθμό των ολοκληρωμένων εργασιών, τον αριθμό των εναπομείναντων, και την εκτίμηση της γραμμής βάσης για το πόσες θα ολοκληρώνονταν σε αυτό το σημείο του έργου.

### CashFlow {#CashFlow}
```
public static final int CashFlow
```


Εμφανίζει τα κόστη και τα συσσωρευμένα κόστη ανά τρίμηνο για όλες τις εργασίες υψηλότερου επιπέδου.

### CostOverruns {#CostOverruns}
```
public static final int CostOverruns
```


Εμφανίζει τη διακύμανση κόστους ανά εργασία και πόρο.

### CostOverview {#CostOverview}
```
public static final int CostOverview
```


Εμφανίζει τις ημερομηνίες έναρξης και λήξης του έργου, το τρέχον προγραμματισμένο και εναπομείναν κόστος, το % ολοκλήρωσης και τις τιμές κόστους για εργασίες υψηλότερου επιπέδου.

### CriticalTasks {#CriticalTasks}
```
public static final int CriticalTasks
```


Εμφανίζει τις εργασίες του έργου που είναι κρίσιμες.

### LateTasks {#LateTasks}
```
public static final int LateTasks
```


Εμφανίζει τις εργασίες του έργου που είναι καθυστερημένες.

### Milestones {#Milestones}
```
public static final int Milestones
```


Εμφανίζει ορόσημα που είναι καθυστερημένα, επερχόμενα και ολοκληρωμένα.

### OverallocatedResources {#OverallocatedResources}
```
public static final int OverallocatedResources
```


Εμφανίζει τον αριθμό των εναπομείναντων ωρών εργασίας για υπερκατανεμημένους πόρους.

### ProjectOverview {#ProjectOverview}
```
public static final int ProjectOverview
```


Εμφανίζει την ημερομηνία έναρξης και λήξης του project\u2019s, το ποσοστό της διάρκειας που\u2019s ολοκληρώθηκε, το ποσοστό ολοκλήρωσης για εργασίες ανώτερου επιπέδου και τα επερχόμενα ορόσημα.

### ResourceCostOverview {#ResourceCostOverview}
```
public static final int ResourceCostOverview
```


Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν κόστος ανά πόρο.

### ResourceOverview {#ResourceOverview}
```
public static final int ResourceOverview
```


Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν έργο ανά πόρο.

### SlippingTasks {#SlippingTasks}
```
public static final int SlippingTasks
```


Εμφανίζει εργασίες που πρέπει να ολοκληρωθούν μετά τις ημερομηνίες λήξης της γραμμής βάσης (η γραμμή βάσης πρέπει να είναι setInternal).

### TaskCostOverview {#TaskCostOverview}
```
public static final int TaskCostOverview
```


Εμφανίζει τη γραμμή βάσης, το πραγματικό και το εναπομείναν κόστος όλων των εργασιών ανώτερου επιπέδου.

### UpcomingTask {#UpcomingTask}
```
public static final int UpcomingTask
```


Εμφανίζει εργασίες που λήγουν κατά τη διάρκεια της τρέχουσας εβδομάδας και εργασίες που ξεκινούν κατά τη διάρκεια της τρέχουσας εβδομάδας.

### WorkOverview {#WorkOverview}
```
public static final int WorkOverview
```


Εμφανίζει τη γραμμή βάσης, το πραγματικό, το εναπομείναν έργο για κάθε εργασία ανώτερου επιπέδου και εργασία για πόρους εργασίας.

