---
title: "Έργο"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα έργο."
type: docs
weight: 220
url: /el/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Αναπαριστά ένα έργο.

--------------------

Η **Project** είναι μια κεντρική κλάση στη βιβλιοθήκη Aspose.Tasks.

Μπορεί κανείς να χρησιμοποιήσει την **Project** για να διαβάσει μία από τις υποστηριζόμενες μορφές διαχείρισης έργου: MPP, MPT, MPX, XML.

Για να φορτώσετε ένα υπάρχον έγγραφο σε οποιαδήποτε από τις υποστηριζόμενες μορφές, περάστε ένα όνομα αρχείου ή μια ροή σε έναν από τους κατασκευαστές της **Project**. Για να δημιουργήσετε ένα κενό έργο, καλέστε τον κατασκευαστή χωρίς παραμέτρους.

Χρησιμοποιήστε μία από τις υπερφορτώσεις της μεθόδου Save για να αποθηκεύσετε το έργο σε οποιαδήποτε από τις μορφές του [SaveFileFormat](../../com.aspose.tasks/savefileformat): Primavera: P6 XML, PM XER· Microsoft Excel: XLSX, XML· Fixed Layout: PDF· Images: JPEG, PNG, BMP, TIFF, SVG· Text: TXT· Others: HTML.

Για να εκτυπώσετε το έργο, χρησιμοποιήστε μία από τις υπερφορτώσεις της μεθόδου [print()](../../com.aspose.tasks/project\#print--).

Η **Project** αποθηκεύει πληροφορίες σε όλο το έργο, όπως `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), και `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). Τα περισσότερα από αυτά τα αντικείμενα είναι προσβάσιμα μέσω των αντίστοιχων ιδιοτήτων της κλάσης **Project**.

Η **Project** είναι μια ριζική οντότητα που περιέχει σημεία εισόδου για τη διαχείριση άλλων οντοτήτων έργου, όπως [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) και [Calendar](../../com.aspose.tasks/calendar).

Οι οντότητες **Project** μπορούν να προσπελαστούν μέσω τυποποιημένων συλλογών, για παράδειγμα `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), κλπ.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Project()](#Project--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο προστατευμένο με κωδικό (υπάρχον αρχείο mpp ή mpt). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από τη ροή με το καθορισμένο στιγμιότυπο της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από μια ροή. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο MPP ή MPT) με το καθορισμένο στιγμιότυπο της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) για ανάγνωση δεδομένων από μια βάση δεδομένων που καθορίζεται από το αντικείμενο της κλάσης [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt) με την καθορισμένη παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από τη ροή με την καθορισμένη παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε ένα άλλο έργο. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε ένα άλλο έργο. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Αναπαράγει αναδρομικά όλες τις εργασίες του έργου, συμπεριλαμβανομένης της ριζικής εργασίας. |
| [getActualsInSync()](#getActualsInSync--) | Λαμβάνει μια τιμή που υποδεικνύει αν το ActualsInSync είναι ορισμένο ή όχι. |
| [getAdminProject()](#getAdminProject--) | Λαμβάνει μια τιμή που υποδεικνύει αν το AdminProject είναι ορισμένο ή όχι. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Λαμβάνει μια τιμή που υποδεικνύει αν το AreEditableActualCosts είναι ορισμένο ή όχι. |
| [getAuthor()](#getAuthor--) | Λαμβάνει την τιμή του Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Λαμβάνει μια τιμή που υποδεικνύει αν το AutoAddNewResourcesAndTasks είναι ορισμένο ή όχι. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Λαμβάνει αν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία της ανάθεσης και τους ρυθμούς των πόρων. |
| [getAutolink()](#getAutolink--) | Λαμβάνει μια τιμή που υποδεικνύει αν το Autolink είναι ορισμένο ή όχι. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Λαμβάνει την τιμή του BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Επιστρέφει το χρόνο αποθήκευσης της βάσης. |
| [getBuiltInProps()](#getBuiltInProps--) | Λαμβάνει τη συλλογή ενσωματωμένων ιδιοτήτων του έργου. |
| [getCalculationMode()](#getCalculationMode--) | Λαμβάνει τη λειτουργία υπολογισμού ενός έργου. |
| [getCalendar()](#getCalendar--) | Λαμβάνει μια τιμή του Calendar. |
| [getCalendars()](#getCalendars--) | Λαμβάνει το αντικείμενο [CalendarCollection](../../com.aspose.tasks/calendarcollection) αυτής της παρουσίασης του Project. |
| [getCategory()](#getCategory--) | Λαμβάνει την τιμή του Category. |
| [getComments()](#getComments--) | Λαμβάνει την τιμή του Comments. |
| [getCompany()](#getCompany--) | Λαμβάνει την τιμή του Company. |
| [getCreationDate()](#getCreationDate--) | Λαμβάνει την τιμή του CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | Λαμβάνει μια συλλογή που περιέχει μια λίστα κρίσιμων εργασιών που αποτελούν την Κρίσιμη Διαδρομή αυτού του έργου. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Οι εργασίες θεωρούνται κρίσιμες από το MS Project εάν το συνολικό περιθώριο είναι μικρότερο ή ίσο με αυτόν τον αριθμό ημερών. |
| [getCurrencyCode()](#getCurrencyCode--) | Λαμβάνει την τιμή του CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Λαμβάνει τιμή του CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Λαμβάνει τιμή του CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Λαμβάνει τιμή του CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Λαμβάνει τιμή του CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Λαμβάνει τιμή του CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Λαμβάνει τη συλλογή προσαρμοσμένων ιδιοτήτων του έργου. |
| [getDateFormat()](#getDateFormat--) | Λαμβάνει τιμή του DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Λαμβάνει τιμή του DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Λαμβάνει τιμή του DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Λαμβάνει τιμή του DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Λαμβάνει τιμή του DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Λαμβάνει τιμή του DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Λαμβάνει τιμή του DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Λαμβάνει τιμή του DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Λαμβάνει τιμή του DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Λαμβάνει την προεπιλεγμένη προβολή του έργου. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Λαμβάνει το στιγμιότυπο της κλάσης [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) που αντιπροσωπεύει μια συλλογή των προεπιλεγμένων ημερών εργασίας της εβδομάδας του έργου και των ωρών εργασίας. |
| [getDisplayOptions()](#getDisplayOptions--) | Λαμβάνει ένα στιγμιότυπο της κλάσης [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Λαμβάνει το αντικείμενο [Duration](../../com.aspose.tasks/duration) με τον καθορισμένο αριθμό μονάδων και την προεπιλεγμένη μορφή διάρκειας που ορίζεται στις ρυθμίσεις του έργου [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Λαμβάνει το αντικείμενο [Duration](../../com.aspose.tasks/duration) με τον καθορισμένο αριθμό μονάδων [TimeUnitType](../../com.aspose.tasks/timeunittype). |
| [getDurationFormat()](#getDurationFormat--) | Λαμβάνει τιμή του DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Λαμβάνει τιμή του EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Λαμβάνει το αντικείμενο ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Λαμβάνει τιμή του ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Λαμβάνει τιμή του FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το FiscalYearStart είναι ορισμένο ή όχι. |
| [getFyStartDate()](#getFyStartDate--) | Λαμβάνει μια τιμή του FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Λαμβάνει τις ρυθμίσεις παγκοσμιοποίησης (συγκεκριμένες για τη γλώσσα) του έργου. |
| [getGuid()](#getGuid--) | Λαμβάνει μια τιμή του Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το HonorConstraints είναι ορισμένο ή όχι. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Λαμβάνει μια τιμή του HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το InsertedProjectsLikeSummary είναι ορισμένο ή όχι. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled είναι ορισμένο ή όχι. |
| [getKeywords()](#getKeywords--) | Λαμβάνει μια τιμή του Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Λαμβάνει μια τιμή του LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Λαμβάνει μια τιμή του LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Λαμβάνει μια τιμή του LastSaved. |
| [getManager()](#getManager--) | Λαμβάνει μια τιμή του Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MicrosoftProjectServerURL είναι ορισμένο ή όχι. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Λαμβάνει μια τιμή του MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Λαμβάνει μια τιμή του MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveCompletedEndsBack είναι ορισμένο ή όχι. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveCompletedEndsForward είναι ορισμένο ή όχι. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveRemainingStartsBack είναι ορισμένο ή όχι. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveRemainingStartsForward είναι ορισμένο ή όχι. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το MultipleCriticalPaths είναι ορισμένο ή όχι. |
| [getName()](#getName--) | Λαμβάνει μια τιμή του Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Λαμβάνει μια τιμή του NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksAreManual είναι ορισμένο ή όχι. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksEffortDriven είναι ορισμένο ή όχι. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksEstimated είναι ορισμένο ή όχι. |
| [getOleObjects()](#getOleObjects--) | Λαμβάνει μια συλλογή που περιέχει τις περιπτώσεις της κλάσης [OleObject](../../com.aspose.tasks/oleobject) η οποία είναι συνδεδεμένη ή ενσωματωμένη σε αυτό το αρχείο έργου. |
| [getOutlineCodes()](#getOutlineCodes--) | Λαμβάνει το αντικείμενο OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το προεπιλεγμένο [Timescale](../../com.aspose.tasks/timescale)(Days). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοθείσες [SaveOptions](../../com.aspose.tasks/saveoptions). |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την δοθείσα [Timescale](../../com.aspose.tasks/timescale) και το [PresentationFormat](../../com.aspose.tasks/presentationformat). |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την δοθείσα [Timescale](../../com.aspose.tasks/timescale) και το [PageSize](../../com.aspose.tasks/pagesize). |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την δοθείσα [Timescale](../../com.aspose.tasks/timescale), το [PresentationFormat](../../com.aspose.tasks/presentationformat) και το εύρος ημερομηνιών. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το προεπιλεγμένο [Timescale](../../com.aspose.tasks/timescale)(Days) και την δοθείσα [PresentationFormat](../../com.aspose.tasks/presentationformat) |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την δοθείσα [Timescale](../../com.aspose.tasks/timescale). |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Επιστρέφει μια συλλογή συνδέσμων εργασιών που είναι προκάτοχοι της καθορισμένης εργασίας. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα έργο που διαβάστηκε από αρχείο Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Λαμβάνει μια τιμή που υποδεικνύει αν το ProjectExternallyEdited είναι ορισμένο ή όχι. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Λαμβάνει πληροφορίες αρχείου έργου από τη ροή. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Διαβάζει πληροφορίες αρχείου έργου από το αρχείο. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Λαμβάνει μια τιμή που υποδεικνύει αν το RemoveFileProperties είναι ορισμένο ή όχι. |
| [getResourceAssignments()](#getResourceAssignments--) | Λαμβάνει το αντικείμενο ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | Λαμβάνει όλους τους ορισμούς φίλτρων βάσει πόρων. |
| [getResourceGroups()](#getResourceGroups--) | Λαμβάνει όλους τους ορισμούς ομάδων βάσει πόρων. |
| [getResources()](#getResources--) | Λαμβάνει το αντικείμενο ResourceCollection. |
| [getRevision()](#getRevision--) | Λαμβάνει μια τιμή του Revision. |
| [getRootTask()](#getRootTask--) | Λαμβάνει τη ρίζα του δέντρου των εργασιών. |
| [getSaveVersion()](#getSaveVersion--) | Λαμβάνει μια τιμή του SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Λαμβάνει μια τιμή που υποδεικνύει αν το ScheduleFromStart είναι ορισμένο ή όχι. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Λαμβάνει μια τιμή που υποδεικνύει αν το ShowProjectSummaryTask είναι ορισμένο ή όχι. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Λαμβάνει μια τιμή που υποδεικνύει αν το SplitsInProgressTasks είναι ορισμένο ή όχι. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Λαμβάνει μια τιμή που υποδεικνύει αν το SpreadActualCost είναι ορισμένο ή όχι. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το SpreadPercentComplete είναι ορισμένο ή όχι. |
| [getStartDate()](#getStartDate--) | Λαμβάνει μια τιμή του StartDate. |
| [getStatusDate()](#getStatusDate--) | Λαμβάνει μια τιμή του StatusDate. |
| [getSubject()](#getSubject--) | Λαμβάνει μια τιμή του Subject. |
| [getTables()](#getTables--) | Λαμβάνει μια λίστα από αντικείμενα [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | Λαμβάνει όλους τους ορισμούς φίλτρων βάσει εργασιών. |
| [getTaskGroups()](#getTaskGroups--) | Λαμβάνει όλους τους ορισμούς ομάδων βάσει εργασιών. |
| [getTaskLinks()](#getTaskLinks--) | Λαμβάνει το αντικείμενο [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το TaskUpdatesResource είναι ορισμένο ή όχι. |
| [getTemplate()](#getTemplate--) | Λαμβάνει μια τιμή του Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Λαμβάνει μια τιμή του TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Λαμβάνει μια τιμή του TimescaleStart. |
| [getTitle()](#getTitle--) | Λαμβάνει μια τιμή του Title. |
| [getUid()](#getUid--) | Λαμβάνει μια τιμή του Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το UpdateManuallyScheduledTasksWhenEditingLinks είναι ορισμένο ή όχι. |
| [getVbaProject()](#getVbaProject--) | Λαμβάνει μια παρουσία της κλάσης `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | Λαμβάνει μια λίστα από αντικείμενα [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Λαμβάνει τον ορισμό κώδικα WBS για το έργο. |
| [getWeekStartDay()](#getWeekStartDay--) | Λαμβάνει μια τιμή του WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Λαμβάνει το αντικείμενο [Duration](../../com.aspose.tasks/duration) με την καθορισμένη τιμή `double` και την προεπιλεγμένη μορφή εργασίας. |
| [getWorkFormat()](#getWorkFormat--) | Λαμβάνει μια τιμή του WorkFormat. |
| [print()](#print--) | Εκτυπώνει το έργο στον προεπιλεγμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Εκτυπώνει το έργο στον προεπιλεγμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή και προσαρμοσμένες επιλογές αποθήκευσης χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή και προσαρμοσμένες επιλογές αποθήκευσης χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή, προσαρμοσμένες επιλογές αποθήκευσης και το καθορισμένο όνομα εγγράφου χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [print(String printerName)](#print-java.lang.String-) | Εκτυπώνει το έργο στον καθορισμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης. |
| [recalculate()](#recalculate--) | Αναπρογραμματίζει όλα τα ids εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις πρώιμες/αργές ημερομηνίες, υπολογίζει τα slacks, την εργασία και τα πεδία κόστους. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Αναπρογραμματίζει όλα τα ids εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις πρώιμες/αργές ημερομηνίες, υπολογίζει τα slacks, την εργασία και τα πεδία κόστους με προαιρετική επικύρωση. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Επαναϋπολογίζει το Id, το Start και το Finish των πόρων. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Επαναϋπολογίζει το Start και το Finish των πόρων. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Καταργεί τις μη έγκυρες εκχωρήσεις πόρων από τη λίστα εκχωρήσεων πόρων του έργου. |
| [renumberWBSCode()](#renumberWBSCode--) | Αριθμεί ξανά τον κωδικό WBS όλων των εργασιών. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Αριθμεί ξανά τον κωδικό WBS των περασμένων εργασιών. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Αναπρογραμματίζει την ατελή εργασία του έργου ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Αναπρογραμματίζει την ατελή εργασία για μια καθορισμένη λίστα εργασιών ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Αποθηκεύει το έργο σε ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Αποθηκεύει τα δεδομένα του έργου στη ροή. |
| [save(String filename)](#save-java.lang.String-) | Αποθηκεύει τα δεδομένα του έργου στο αρχείο σε μορφή mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Αποθηκεύει το έγγραφο σε αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Αποθηκεύει τα δεδομένα του έργου στο αρχείο. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Αποθηκεύει το έργο ως πρότυπο σε μια καθορισμένη ροή. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Αποθηκεύει το έργο ως πρότυπο σε μια καθορισμένη ροή. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Αποθηκεύει το έργο ως πρότυπο στη καθορισμένη διαδρομή αρχείου. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Αποθηκεύει το έργο ως πρότυπο. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Αποθηκεύει την αναφορά επισκόπησης του έργου στη ροή. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Αποθηκεύει την αναφορά του έργου του καθορισμένου τύπου στη καθορισμένη ροή. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Αποθηκεύει την αναφορά επισκόπησης του έργου σε αρχείο PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Αποθηκεύει την αναφορά του έργου του καθορισμένου τύπου σε μορφή PDF στη καθορισμένη διαδρομή αρχείου. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Συλλέγει επαναληπτικά όλες τις θυγατρικές εργασίες της ριζικής εργασίας. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το ActualsInSync είναι ορισμένο ή όχι. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το AdminProject είναι ορισμένο ή όχι. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το AreEditableActualCosts είναι ορισμένο ή όχι. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ορίζει μια τιμή του Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το AutoAddNewResourcesAndTasks είναι ορισμένο ή όχι. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Ορίζει εάν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία της ανάθεσης και τις τιμές των πόρων. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το Autolink είναι ορισμένο ή όχι. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Αποθηκεύει τα πεδία βάσης στο καθορισμένο baseline για ολόκληρο το έργο. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Αποθηκεύει τα πεδία βάσης στο καθορισμένο baseline για τις επιλεγμένες εργασίες. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Ορίζει μια τιμή του BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Ορίζει το χρόνο αποθήκευσης της βάσης. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Ορίζει τη λειτουργία υπολογισμού ενός έργου. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Ορίζει μια τιμή για το Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Ορίζει μια τιμή της Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Ορίζει μια τιμή των Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Ορίζει μια τιμή της Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Ορίζει μια τιμή του CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Οι εργασίες θεωρούνται κρίσιμες από το MS Project εάν το συνολικό περιθώριο είναι μικρότερο ή ίσο με αυτόν τον αριθμό ημερών. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Ορίζει μια τιμή του CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Ορίζει μια τιμή του CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Ορίζει μια τιμή του CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Ορίζει μια τιμή του CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Ορίζει μια τιμή του CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Ορίζει μια τιμή του CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Ορίζει μια τιμή του DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Ορίζει μια τιμή του DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Ορίζει μια τιμή του DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Ορίζει μια τιμή του DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Ορίζει μια τιμή του DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Ορίζει μια τιμή του DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Ορίζει μια τιμή του DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Ορίζει μια τιμή του DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Ορίζει μια τιμή του DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Ορίζει την προεπιλεγμένη προβολή του έργου. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Ορίζει μια τιμή του DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Ορίζει μια τιμή του EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Ορίζει μια τιμή του ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Ορίζει μια τιμή του FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το FiscalYearStart είναι ορισμένο ή όχι. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Ορίζει μια τιμή του FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Ορίζει τις ρυθμίσεις παγκοσμιοποίησης (συγκεκριμένες για τη γλώσσα) του έργου. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Ορίζει μια τιμή για το Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το HonorConstraints είναι ορισμένο ή όχι. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Ορίζει μια τιμή του HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το InsertedProjectsLikeSummary είναι ορισμένο ή όχι. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled είναι ορισμένο ή όχι. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Ορίζει μια τιμή του Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Ορίζει μια τιμή του LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Ορίζει μια τιμή του LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Ορίζει μια τιμή του LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Ορίζει μια τιμή του Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το MicrosoftProjectServerURL είναι ορισμένο ή όχι. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Ορίζει μια τιμή του MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Ορίζει μια τιμή του MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το MoveCompletedEndsBack είναι ορισμένο ή όχι. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν MoveCompletedEndsForward είναι ορισμένο ή όχι. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν MoveRemainingStartsBack είναι ορισμένο ή όχι. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν MoveRemainingStartsForward είναι ορισμένο ή όχι. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν MultipleCriticalPaths είναι ορισμένο ή όχι. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει μια τιμή του Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Ορίζει μια τιμή του NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν NewTasksAreManual είναι ορισμένο ή όχι. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν NewTasksEffortDriven είναι ορισμένο ή όχι. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν NewTasksEstimated είναι ορισμένο ή όχι. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν ProjectExternallyEdited είναι ορισμένο ή όχι. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν RemoveFileProperties είναι ορισμένο ή όχι. |
| [setRevision(int value)](#setRevision-int-) | Ορίζει μια τιμή του Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Ορίζει μια τιμή του SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν ScheduleFromStart είναι ορισμένο ή όχι. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ShowProjectSummaryTask είναι ορισμένο ή όχι. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν SplitsInProgressTasks είναι ορισμένο ή όχι. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν SpreadActualCost είναι ορισμένο ή όχι. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν SpreadPercentComplete είναι ορισμένο ή όχι. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ορίζει μια τιμή του StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Ορίζει μια τιμή του StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Ορίζει μια τιμή του Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν TaskUpdatesResource είναι ορισμένο ή όχι. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Ορίζει μια τιμή του Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Ορίζει μια τιμή του TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Ορίζει μια τιμή του TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Ορίζει μια τιμή του Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Ορίζει μια τιμή του Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το UpdateManuallyScheduledTasksWhenEditingLinks είναι ορισμένο ή όχι. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Ορίζει τον ορισμό κώδικα WBS για το έργο. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Ορίζει μια τιμή του WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Ορίζει μια τιμή του WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Ενημερώνει όλη τη δουλειά ως ολοκληρωμένη μέχρι μια καθορισμένη ημερομηνία για ολόκληρο το έργο. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Ενημερώνει όλη τη δουλειά ως ολοκληρωμένη μέχρι μια καθορισμένη ημερομηνία για τη συγκεκριμένη λίστα εργασιών. |
### Project() {#Project--}
```
public Project()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο προστατευμένο με κωδικό (υπάρχον αρχείο mpp ή mpt).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | java.lang.String | Διαδρομή προς το πρότυπο για δημιουργία του έργου. |
|  | protectionPassword | java.lang.String | Κωδικός προστασίας. |

--------------------

Η ανάγνωση αρχείων προστατευμένων με κωδικό υποστηρίζεται επί του παρόντος μόνο για μορφή αρχείου MSP 2003. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | java.lang.String | Διαδρομή προς το πρότυπο για δημιουργία του έργου. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από τη ροή με το καθορισμένο στιγμιότυπο της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | Ροή του Project java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | η καθορισμένη παρουσία της [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)class που επιτρέπει την προσαρμογή της ανάγνωσης των μορφών Primavera (XER ή XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | java.lang.String | Διαδρομή προς το πρότυπο για δημιουργία του έργου. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | η καθορισμένη μέθοδος callback για τη διαχείριση σφαλμάτων ανάλυσης xml. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από μια ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream για φόρτωση προτύπου από. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο MPP ή MPT) με το καθορισμένο στιγμιότυπο της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | java.lang.String | Διαδρομή προς το πρότυπο για δημιουργία του έργου από |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | η καθορισμένη παρουσία της [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) για ανάγνωση δεδομένων από μια βάση δεδομένων που καθορίζεται από το αντικείμενο της κλάσης [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | η καθορισμένη παρουσία της [DbSettings](../../com.aspose.tasks/dbsettings) class. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream για φόρτωση προτύπου από. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | η καθορισμένη μέθοδος callback για τη διαχείριση σφαλμάτων ανάλυσης xml. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream για φόρτωση προτύπου από. |
|  | protectionPassword | java.lang.String | Κωδικός προστασίας. |

--------------------

Η ανάγνωση αρχείων προστατευμένων με κωδικό υποστηρίζεται επί του παρόντος μόνο για μορφή αρχείου MSP 2003. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt) με την καθορισμένη παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | java.lang.String | Διαδρομή προς το πρότυπο για δημιουργία του έργου από |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | η καθορισμένη παρουσία της [LoadOptions](../../com.aspose.tasks/loadoptions) class. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Project](../../com.aspose.tasks/project) από τη ροή με την καθορισμένη παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | java.io.InputStream | Ροή του Project java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | η καθορισμένη παρουσία της [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Prj](../../com.aspose.tasks/prj) για λήψη του κλειδιού ιδιότητας. |

**Returns:**
T - η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Prj](../../com.aspose.tasks/prj) για λήψη του κλειδιού ιδιότητας. |
| val | T | η τιμή. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε ένα άλλο έργο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Άλλο έργο για αντιγραφή δεδομένων. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε ένα άλλο έργο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Άλλο έργο για αντιγραφή δεδομένων. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Επιλογές αντιγραφής για έλεγχο της διαδικασίας αντιγραφής. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Αναπαράγει αναδρομικά όλες τις εργασίες του έργου, συμπεριλαμβανομένης της ριζικής εργασίας.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable που μπορεί να χρησιμοποιηθεί για την επανάληψη σε όλες τις εργασίες του έργου.

--------------------

Παρέχει έναν πιο ελαφρύ τρόπο για την επανάληψη στις εργασίες σε σύγκριση με τη μέθοδο [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) καθώς δεν διανέμει μνήμη για όλες τις εργασίες.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το ActualsInSync είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το AdminProject είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το AreEditableActualCosts είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Λαμβάνει την τιμή του Author.

**Returns:**
java.lang.String - μια τιμή του Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το AutoAddNewResourcesAndTasks είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Λαμβάνει αν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία της ανάθεσης και τους ρυθμούς των πόρων.

**Returns:**
boolean - αν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία της ανάθεσης και τους ρυθμούς πόρων.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το Autolink είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Λαμβάνει την τιμή του BaselineForEarnedValue.

**Returns:**
int - μια τιμή του BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Επιστρέφει την ώρα αποθήκευσης της βάσης. Επιστρέφει DateTime.MinValue (00:00:00.0000000 UTC, 1η Ιανουαρίου 0001) εάν η βάση δεν αποθηκεύτηκε.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| baselineNumber | int | Ο αριθμός της βάσης [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - Η τελευταία ημερομηνία και ώρα αποθήκευσης της βάσης.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Λαμβάνει τη συλλογή ενσωματωμένων ιδιοτήτων του έργου.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Λαμβάνει τη λειτουργία υπολογισμού ενός έργου. Μπορεί να είναι μία από τις τιμές της αρίθμησης `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - λειτουργία υπολογισμού ενός έργου.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Λαμβάνει μια τιμή του Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Λαμβάνει το αντικείμενο [CalendarCollection](../../com.aspose.tasks/calendarcollection) αυτής της παρουσίασης του Project.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Λαμβάνει την τιμή του Category.

**Returns:**
java.lang.String - μια τιμή του Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Λαμβάνει την τιμή του Comments.

**Returns:**
java.lang.String - μια τιμή του Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Λαμβάνει την τιμή του Company.

**Returns:**
java.lang.String - μια τιμή του Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Λαμβάνει την τιμή του CreationDate.

**Returns:**
java.util.Date - μια τιμή του CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Λαμβάνει μια συλλογή που περιέχει μια λίστα κρίσιμων εργασιών που αποτελούν την Κρίσιμη Διαδρομή αυτού του έργου.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Αυτή είναι μια λειτουργία O(n), όπου n είναι ο αριθμός των εργασιών στο έργο.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Οι εργασίες θεωρούνται κρίσιμες από το MS Project εάν το συνολικό περιθώριο είναι μικρότερο ή ίσο με αυτόν τον αριθμό ημερών.

**Returns:**
int - η μέγιστη τιμή του συνολικού χρόνου ελεύθερου (σε ημέρες) κατά την οποία μια εργασία θεωρείται κρίσιμη
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Λαμβάνει την τιμή του CurrencyCode.

**Returns:**
java.lang.String - μια τιμή του CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Λαμβάνει τιμή του CurrencyDigits.

**Returns:**
int - μια τιμή του CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Λαμβάνει τιμή του CurrencySymbol.

**Returns:**
java.lang.String - μια τιμή του CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Λαμβάνει τιμή του CurrencySymbolPosition.

**Returns:**
int - μια τιμή του CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Λαμβάνει τιμή του CurrentDate.

**Returns:**
java.util.Date - μια τιμή του CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Λαμβάνει τιμή του CustomDateFormat.

**Returns:**
java.lang.String - μια τιμή του CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Λαμβάνει τη συλλογή προσαρμοσμένων ιδιοτήτων του έργου.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Λαμβάνει τιμή του DateFormat.

**Returns:**
int - μια τιμή του DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Λαμβάνει τιμή του DaysPerMonth.

**Returns:**
int - μια τιμή του DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Λαμβάνει τιμή του DefaultFinishTime.

**Returns:**
java.util.Date - μια τιμή του DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Λαμβάνει τιμή του DefaultFixedCostAccrual.

**Returns:**
int - μια τιμή του DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Λαμβάνει τιμή του DefaultOvertimeRate.

**Returns:**
double - μια τιμή του DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Λαμβάνει τιμή του DefaultStandardRate.

**Returns:**
double - μια τιμή του DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Λαμβάνει τιμή του DefaultStartTime.

**Returns:**
java.util.Date - μια τιμή του DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Λαμβάνει τιμή του DefaultTaskEVMethod.

**Returns:**
int - μια τιμή του DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Λαμβάνει τιμή του DefaultTaskType.

**Returns:**
int - μια τιμή του DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Λαμβάνει την προεπιλεγμένη προβολή του έργου.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Λαμβάνει το στιγμιότυπο της κλάσης [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) που αντιπροσωπεύει μια συλλογή των προεπιλεγμένων ημερών εργασίας της εβδομάδας του έργου και των ωρών εργασίας.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Τα δεδομένα περιέχονται μόνο σε αρχεία mpp (όχι σε xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Λαμβάνει ένα στιγμιότυπο της κλάσης [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Λαμβάνει το αντικείμενο [Duration](../../com.aspose.tasks/duration) με τον καθορισμένο αριθμό μονάδων και την προεπιλεγμένη μορφή διάρκειας που ορίζεται στις ρυθμίσεις του έργου [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | val | double | καθορισμένος αριθμός μονάδων. |

--------------------

Αυτή η μέθοδος πρέπει να χρησιμοποιείται προσεκτικά επειδή επιστρέφει διαφορετικές διάρκειες ανάλογα με τη ρύθμιση Project.DurationFormat. Για παράδειγμα, το GetWork(1.0) θα επιστρέψει 1 ώρα όταν το Project.DurationFormat είναι TimeUnitType.Hour ή 1 ημέρα αν το Project.DurationFormat είναι TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Λαμβάνει το αντικείμενο [Duration](../../com.aspose.tasks/duration) με τον καθορισμένο αριθμό μονάδων [TimeUnitType](../../com.aspose.tasks/timeunittype).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | double | καθορισμένος αριθμός μονάδων. |
| μονάδα χρόνου | byte | καθορισμένη τιμή του TimeUnitType. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Λαμβάνει τιμή του DurationFormat.

**Returns:**
byte - μια τιμή του DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Λαμβάνει τιμή του EarnedValueMethod.

**Returns:**
int - μια τιμή του EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Λαμβάνει το αντικείμενο ExtendedAttributeDefinitionCollection. Η συλλογή των ορισμών εκτεταμένων χαρακτηριστικών (προσαρμοσμένων πεδίων) που σχετίζονται με ένα έργο.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Λαμβάνει τιμή του ExtendedCreationDate.

**Returns:**
java.util.Date - μια τιμή του ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Λαμβάνει τιμή του FinishDate.

**Returns:**
java.util.Date - μια τιμή του FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το FiscalYearStart είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Λαμβάνει μια τιμή του FyStartDate.

**Returns:**
int - μια τιμή του FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Λαμβάνει τις ρυθμίσεις παγκοσμιοποίησης (συγκεκριμένες για τη γλώσσα) του έργου.

Ο συνιστώμενος τρόπος είναι η χρήση κυριολεκτικών ή μορφών ανεξάρτητων από την πολιτισμική ρύθμιση σε όλο το έργο. Ωστόσο, εάν ένα έργο χρησιμοποιεί κυριολεκτικά ειδικά για έναν πολιτισμό, αυτή η κλάση μπορεί να χρησιμοποιηθεί για να βοηθήσει τη μηχανή υπολογισμού να αναλύσει αυτά τα κυριολεκτικά.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Λαμβάνει μια τιμή του Guid.

**Returns:**
java.util.UUID - μια τιμή του Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το HonorConstraints είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Λαμβάνει μια τιμή του HyperlinkBase.

**Returns:**
java.lang.String - μια τιμή του HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το InsertedProjectsLikeSummary είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Λαμβάνει μια τιμή του Keywords.

**Returns:**
java.lang.String - μια τιμή του Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Λαμβάνει μια τιμή του LastAuthor.

**Returns:**
java.lang.String - μια τιμή του LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Λαμβάνει μια τιμή του LastPrinted.

**Returns:**
java.util.Date - μια τιμή του LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Λαμβάνει μια τιμή του LastSaved.

**Returns:**
java.util.Date - μια τιμή του LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Λαμβάνει μια τιμή του Manager.

**Returns:**
java.lang.String - μια τιμή του Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MicrosoftProjectServerURL είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Λαμβάνει μια τιμή του MinutesPerDay.

**Returns:**
int - μια τιμή του MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Λαμβάνει μια τιμή του MinutesPerWeek.

**Returns:**
int - μια τιμή του MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveCompletedEndsBack είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveCompletedEndsForward είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveRemainingStartsBack είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MoveRemainingStartsForward είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το MultipleCriticalPaths είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει μια τιμή του Name.

**Returns:**
java.lang.String - μια τιμή του Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Λαμβάνει μια τιμή του NewTaskStartDate.

**Returns:**
int - μια τιμή του NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksAreManual είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksEffortDriven είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το NewTasksEstimated είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Λαμβάνει μια συλλογή που περιέχει τις περιπτώσεις της κλάσης [OleObject](../../com.aspose.tasks/oleobject) η οποία είναι συνδεδεμένη ή ενσωματωμένη σε αυτό το αρχείο έργου.

--------------------

Διαθέσιμο μόνο για μορφή αρχείου mpp. Αυτή η συλλογή είναι μόνο για ανάγνωση εκτός από τη λειτουργία 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Λαμβάνει το αντικείμενο OutlineCodeDefinitionCollection. Η συλλογή των ορισμών κώδικα περιγράμματος που σχετίζονται με ένα έργο.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το προεπιλεγμένο [Timescale](../../com.aspose.tasks/timescale)(Days).

**Returns:**
int - Αριθμός σελίδων που θα αποδοθεί.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοθείσες [SaveOptions](../../com.aspose.tasks/saveoptions).

--------------------

&gt; ```
&gt; Σε αυτό το παράδειγμα η παρουσίαση του HtmlSaveOptions και ο αριθμός των σελίδων στο παραγόμενο HTML γράφεται στην κονσόλα.
&gt; ``````

  [C#]
Project project = new Project(@\"test.mpp\");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
public final int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
public final NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
public final boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
public final NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
public final NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
public final NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
public final Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
public final String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
public final NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
public final String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
public final Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
public final Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
public final String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
public final String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
public final NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
public final int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

