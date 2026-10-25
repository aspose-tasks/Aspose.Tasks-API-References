---
title: "ProjectServerCredentials"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Διαπιστευτήρια που χρησιμοποιούνται για σύνδεση στο Project Online ή σε τοπική παρουσία του Project Server."
type: docs
weight: 225
url: /el/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Διαπιστευτήρια που χρησιμοποιούνται για σύνδεση στο Project Online ή σε τοπική παρουσία του Project Server.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) χρησιμοποιώντας το URL του ιστότοπου SharePoint και έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA (Project Web Access) του SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) χρησιμοποιώντας το URL του ιστότοπου SharePoint, το όνομα χρήστη και τον κωδικό πρόσβασης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Λαμβάνει το διακριτικό εξουσιοδότησης για την παρουσία του SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | Λαμβάνει το URL του PWA στον ιστότοπο SharePoint ή το URL του τοπικού Project Server. |
| [getUserName()](#getUserName--) | Λαμβάνει το όνομα χρήστη για τον ιστότοπο SharePoint. |
| [toString()](#toString--) | Επιστρέφει μια αναπαράσταση κειμένου αυτής της παρουσίασης. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) χρησιμοποιώντας το URL του ιστότοπου SharePoint και έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA (Project Web Access) του SharePoint.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| siteUrl | java.lang.String | Το URL του API PWA (Project Web Access) του Project Online. |
|  | authToken | java.lang.String | Το διακριτικό εξουσιοδότησης (SPOIDCRL) για τον ιστότοπο PWA (Project Web Access) του SharePoint. |

--------------------

Χρησιμοποιήστε αυτόν τον κατασκευαστή για να συνδεθείτε στο ProjectOnline όταν έχετε ήδη AuthToken για τον ιστότοπο SharePoint Online σας. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) χρησιμοποιώντας το URL του ιστότοπου SharePoint, το όνομα χρήστη και τον κωδικό πρόσβασης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| siteUrl | java.lang.String | Το URL του API PWA (Project Web Access) του Project Online. |
| userName | java.lang.String | Το όνομα χρήστη για τον ιστότοπο SharePoint. |
|  | password | java.lang.String | Ο κωδικός πρόσβασης για τον ιστότοπο SharePoint. |

--------------------

Χρησιμοποιήστε αυτόν τον κατασκευαστή για να συνδεθείτε στο ProjectOnline. Παρακαλούμε σημειώστε ότι η παλαιότερη πιστοποίηση πρέπει να είναι ενεργοποιημένη στο Azure portal και στο κέντρο διαχείρισης Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Λαμβάνει το διακριτικό εξουσιοδότησης για την παρουσία του SharePoint.

**Returns:**
java.lang.String - το διακριτικό εξουσιοδότησης για την παρουσία του SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Λαμβάνει το URL του PWA στον ιστότοπο SharePoint ή το URL του τοπικού Project Server. Για παράδειγμα, https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - το URL του PWA στον ιστότοπο SharePoint ή το URL του τοπικού Project Server.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Λαμβάνει το όνομα χρήστη για τον ιστότοπο SharePoint.

**Returns:**
java.lang.String - το όνομα χρήστη για τον ιστότοπο SharePoint.
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει μια αναπαράσταση κειμένου αυτής της παρουσίασης.

**Returns:**
java.lang.String - μια συμβολοσειρά αναπαράστασης αυτής της εμφάνισης.
