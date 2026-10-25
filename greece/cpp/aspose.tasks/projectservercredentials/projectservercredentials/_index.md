---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials κατασκευαστής"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks για C++"
description: "Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ProjectServerCredentials χρησιμοποιώντας τη διεύθυνση URL του ιστότοπου SharePoint και έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για το PWA ( Project"
type: docs
weight: 10
url: /el/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης ProjectServerCredentials χρησιμοποιώντας το URL του ιστότοπου SharePoint και ένα έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA (Project Web Access) του SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| siteUrl | Η διεύθυνση URL του API PWA (Project Web Access) του Project Online. |
| authToken | Το διακριτικό εξουσιοδότησης (SPOIDCRL) για τον ιστότοπο PWA (Project Web Access) του SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ProjectServerCredentials χρησιμοποιώντας τη διεύθυνση URL του ιστότοπου SharePoint, το όνομα χρήστη και τον κωδικό πρόσβασης.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| siteUrl | Η διεύθυνση URL του API PWA (Project Web Access) του Project Online. |
| userName | Το όνομα χρήστη για τον ιστότοπο SharePoint. |
| password | Ο κωδικός πρόσβασης για τον ιστότοπο SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ProjectServerCredentials χρησιμοποιώντας τη διεύθυνση URL του σημείου λήψης Project Web Access και τα διαπιστευτήρια δικτύου.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| siteUrl | Η διεύθυνση URL του σημείου λήψης project web access. |
| διαπιστευτήρια | Τα διαπιστευτήρια που χρησιμοποιούνται για σύνδεση στο σημείο λήψης Project Web Access. |

