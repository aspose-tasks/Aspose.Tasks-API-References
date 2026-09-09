---
title: "FilterCriteria"
second_title: "Aspose.Tasks για Python μέσω .NET API Αναφορά"
description: 
type: docs
weight: 350
url: /el/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP.

Ο τύπος FilterCriteria εκθέτει τα παρακάτω μέλη:
## Κατασκευαστές
| Όνομα | Περιγραφή |
| :- | :- |
| FilterCriteria() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης FilterCriteria |
## Ιδιότητες
| Όνομα | Περιγραφή |
| :- | :- |
| operation | Λαμβάνει ή ορίζει το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο. |
| field | Λαμβάνει ή ορίζει ένα [field](/tasks/python-net/aspose.tasks/filtercriteria/) για αλλαγή. |
| test | Λαμβάνει ή ορίζει τον τύπο σύγκρισης που γίνεται μεταξύ των FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Λαμβάνει τις τιμές αντικειμένου για σύγκριση με την τιμή του πεδίου που καθορίζεται με το FieldName. |
| criteria_rows | Λαμβάνει τη λίστα των θυγατρικών γραμμών [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/).<br/>            Εάν το φίλτρο περιέχει περισσότερες από μία γραμμές κριτηρίου, τότε η επίδραση του τελεστή And είναι ότι τα κριτήρια και για τις δύο γραμμές πρέπει να ικανοποιηθούν ώστε η εργασία ή ο πόρος να εμφανιστούν ως αποτέλεσμα αυτού του φίλτρου.<br/>            Η επίδραση του τελεστή Or είναι ότι τα κριτήρια για τη μία ή την άλλη γραμμή πρέπει να ικανοποιηθούν. |
## Methods
| Όνομα | Περιγραφή |
| :- | :- |
| is_field_value() | Λαμβάνει αν η δεξιά τιμή του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή. |
| set_value_field(value) | Ορίζει το πεδίο του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από το FieldName. |

### Δείτε επίσης

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

