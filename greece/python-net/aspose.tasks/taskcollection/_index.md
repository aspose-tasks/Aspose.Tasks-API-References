---
title: "TaskCollection"
second_title: "Aspose.Tasks για Python μέσω .NET API Αναφορά"
description: 
type: docs
weight: 1140
url: /el/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Αναπαριστά μια συλλογή από αντικείμενα [Task](/tasks/python-net/aspose.tasks/task/).

Ο τύπος TaskCollection εκθέτει τα παρακάτω μέλη:
## Ιδιότητες
| Όνομα | Περιγραφή |
| :- | :- |
| parent_project | Λαμβάνει το γονικό έργο του αντικειμένου TaskCollection. |
## Methods
| Όνομα | Περιγραφή |
| :- | :- |
| add() | Προσθέστε την καθορισμένη εργασία στην παρουσία της κλάσης [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/> Εάν ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως καθυστερήσεις, εργασία και πεδία κόστους, τα IDs και τα επίπεδα περιγράμματος).<br/> Εάν ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το ID της εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος αυτόματα.<br/> Εάν ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου<br/> (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες, υπολογίζει καθυστερήσεις, εργασία και πεδία κόστους, επαναϋπολογίζει τα IDs και τα επίπεδα περιγράμματος). |
| add(task_name) | Προσθέτει μια νέα εργασία στη συλλογή των υποεργασιών. |
| add(task_name, before_task_id) |  |
| add(parameters) | Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο id και στο ίδιο επίπεδο περιγράμματος. |
| to_list() | Μετατρέπει το αντικείμενο TaskCollection σε λίστα αντικειμένων [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Επιστρέφει μια εργασία με το καθορισμένο Uid της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |
| get_by_id(id) | Επιστρέφει μια εργασία με το καθορισμένο Id της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |

### Δείτε επίσης

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

