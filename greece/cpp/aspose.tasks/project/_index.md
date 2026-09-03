---
title: "**Aspose::Tasks::Project** κλάση"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks για C++"
description: "Αντιπροσωπεύει ένα έργο."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/project/
---

## Project class

Αντιπροσωπεύει ένα έργο.

Το **Project** είναι μια κεντρική κλάση στη βιβλιοθήκη **Aspose.Tasks**.

Μπορείτε να χρησιμοποιήσετε το **Project** για να διαβάσετε μία από τις υποστηριζόμενες μορφές διαχείρισης έργων: MPP, MPT, MPX, XML.

Για να φορτώσετε ένα υπάρχον έγγραφο σε οποιαδήποτε από τις υποστηριζόμενες μορφές, περάστε ένα όνομα αρχείου ή μια ροή σε έναν από τους κατασκευαστές του **Project**. Για να δημιουργήσετε ένα κενό έργο, καλέστε τον κατασκευαστή χωρίς παραμέτρους.

Χρησιμοποιήστε μία από τις υπερφορτώσεις της μεθόδου **Save** για να αποθηκεύσετε το έργο σε οποιαδήποτε από τις μορφές **Aspose::Tasks::Saving::SaveFileFormat**: Primavera: P6 XML, PM XER· Microsoft Excel: XLSX, XML· Σταθερή διάταξη: PDF· Εικόνες: JPEG, PNG, BMP, TIFF, SVG· Κείμενο: TXT· Άλλα: HTML.

Το **Project** αποθηκεύει πληροφορίες σε όλο το έργο, όπως **Aspose::Tasks::Project::Views**, **Aspose::Tasks::Project::BuiltInProps**, **Aspose::Tasks::Project::CustomProps** και **Aspose::Tasks::Project::ExtendedAttributes**. Τα περισσότερα από αυτά τα αντικείμενα είναι προσβάσιμα μέσω των αντίστοιχων ιδιοτήτων της κλάσης **Project**.

Το Project είναι μια ριζική οντότητα που περιέχει σημεία εισόδου για τη διαχείριση άλλων οντοτήτων έργου, όπως Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute και Aspose::Tasks::Calendar.

Οι οντότητες Project μπορούν να προσπελαστούν μέσω τυποποιημένων συλλογών, για παράδειγμα Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments, κ.λπ.

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Project (13 overloads)](./project/) | Αρχικοποιεί μια νέα παρουσία της κλάσης Project. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του project σε ένα άλλο project. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Αναπαράγει αναδρομικά όλες τις εργασίες του project, συμπεριλαμβανομένης της ριζικής εργασίας. |
| [Get](./get/) | Επιστρέφει την τιμή στην οποία αντιστοιχεί η ιδιότητα σε αυτό το κοντέινερ. |
| [get_ActualsInSync](./get_actualsinsync/) | Λαμβάνει μια τιμή που υποδεικνύει αν το ActualsInSync είναι ορισμένο ή όχι. |
| [get_AdminProject](./get_adminproject/) | Λαμβάνει μια τιμή που υποδεικνύει αν το AdminProject είναι ορισμένο ή όχι. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Λαμβάνει μια τιμή που υποδεικνύει αν το AreEditableActualCosts είναι ορισμένο ή όχι. |
| [get_Author](./get_author/) | Λαμβάνει μια τιμή του Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Λαμβάνει μια τιμή που υποδεικνύει αν το AutoAddNewResourcesAndTasks είναι ορισμένο ή όχι. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Λαμβάνει αν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογιστούν αυτόματα χρησιμοποιώντας το έργο της ανάθεσης και τους ρυθμούς των πόρων. |
| [get_Autolink](./get_autolink/) | Λαμβάνει μια τιμή που υποδεικνύει αν το Autolink είναι ορισμένο ή όχι. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Λαμβάνει μια τιμή του BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Λαμβάνει τη συλλογή ενσωματωμένων ιδιοτήτων του project. |
| [get_CalculationMode](./get_calculationmode/) | Λαμβάνει τη λειτουργία υπολογισμού ενός project. Μπορεί να είναι μία από τις τιμές της απαρίθμησης CalculationMode. |
| [get_Calendar](./get_calendar/) | Λαμβάνει μια τιμή του Calendar. |
| [get_Calendars](./get_calendars/) | Λαμβάνει το αντικείμενο CalendarCollection αυτής της παρουσίας Project. |
| [get_Category](./get_category/) | Λαμβάνει μια τιμή του Category. |
| [get_Comments](./get_comments/) | Λαμβάνει μια τιμή του Comments. |
| [get_Company](./get_company/) | Λαμβάνει μια τιμή του Company. |
| [get_CreationDate](./get_creationdate/) | Λαμβάνει μια τιμή του CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Λαμβάνει μια συλλογή που περιέχει μια λίστα από κρίσιμες εργασίες που αποτελούν την Κρίσιμη Διαδρομή αυτού του project. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Λαμβάνει μια τιμή του CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Λαμβάνει μια τιμή του CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Λαμβάνει μια τιμή του CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Λαμβάνει μια τιμή του CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Λαμβάνει τιμή του CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Λαμβάνει τιμή του CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Λαμβάνει τιμή του CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Λαμβάνει τη συλλογή προσαρμοσμένων ιδιοτήτων του έργου. |
| [get_DateFormat](./get_dateformat/) | Λαμβάνει τιμή του DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Λαμβάνει τιμή του DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Λαμβάνει τιμή του DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Λαμβάνει τιμή του DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Λαμβάνει τιμή του DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Λαμβάνει τιμή του DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Λαμβάνει τιμή του DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Λαμβάνει τιμή του DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Λαμβάνει τιμή του DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Λαμβάνει την προεπιλεγμένη προβολή του έργου. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Λαμβάνει το στιγμιότυπο της κλάσης WeekDayCollection που αντιπροσωπεύει μια συλλογή των προεπιλεγμένων εβδομαδιαίων εργάσιμων ημερών και ωρών εργασίας του έργου. |
| [get_DisplayOptions](./get_displayoptions/) | Λαμβάνει ένα στιγμιότυπο της κλάσης ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Λαμβάνει τιμή του DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Λαμβάνει τιμή του EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Λαμβάνει το αντικείμενο ExtendedAttributeDefinitionCollection. Η συλλογή των ορισμών επεκταμένων ιδιοτήτων (προσαρμοσμένων πεδίων) που σχετίζονται με ένα έργο. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Λαμβάνει τιμή του ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Λαμβάνει τιμή του FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Λαμβάνει τιμή που υποδεικνύει αν το FiscalYearStart έχει οριστεί ή όχι. |
| [get_FyStartDate](./get_fystartdate/) | Λαμβάνει τιμή του FyStartDate. |
| [get_Guid](./get_guid/) | Λαμβάνει μια τιμή του Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Λαμβάνει τιμή που υποδεικνύει αν το HonorConstraints έχει οριστεί ή όχι. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Λαμβάνει τιμή του HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Λαμβάνει μια τιμή που υποδεικνύει αν το InsertedProjectsLikeSummary είναι ορισμένο ή όχι. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Λαμβάνει μια τιμή που υποδεικνύει αν το KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled είναι ορισμένο ή όχι. |
| [get_Keywords](./get_keywords/) | Λαμβάνει μια τιμή των Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Λαμβάνει μια τιμή του LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Λαμβάνει μια τιμή του LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Λαμβάνει μια τιμή του LastSaved. |
| [get_Manager](./get_manager/) | Λαμβάνει μια τιμή του Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MicrosoftProjectServerURL είναι ορισμένο ή όχι. |
| [get_MinutesPerDay](./get_minutesperday/) | Λαμβάνει μια τιμή του MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Λαμβάνει μια τιμή του MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MoveCompletedEndsBack είναι ορισμένο ή όχι. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MoveCompletedEndsForward είναι ορισμένο ή όχι. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MoveRemainingStartsBack είναι ορισμένο ή όχι. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MoveRemainingStartsForward είναι ορισμένο ή όχι. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Λαμβάνει μια τιμή που υποδεικνύει αν το MultipleCriticalPaths είναι ορισμένο ή όχι. |
| [get_Name](./get_name/) | Λαμβάνει μια τιμή του Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Λαμβάνει μια τιμή που υποδεικνύει αν το NewTasksAreManual είναι ορισμένο ή όχι. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Λαμβάνει μια τιμή που υποδεικνύει αν το NewTasksEffortDriven είναι ορισμένο ή όχι. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Λαμβάνει μια τιμή που υποδεικνύει αν το NewTasksEstimated είναι ορισμένο ή όχι. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Λαμβάνει μια τιμή του NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Λαμβάνει μια συλλογή που περιέχει τις εμφανίσεις της κλάσης OleObject οι οποίες είναι συνδεδεμένες ή ενσωματωμένες σε αυτό το αρχείο έργου. |
| [get_OutlineCodes](./get_outlinecodes/) | Λαμβάνει το αντικείμενο OutlineCodeDefinitionCollection. Η συλλογή των ορισμών κώδικα περιγράμματος που σχετίζονται με ένα έργο. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα έργο που διαβάζεται από αρχείο Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Λαμβάνει μια τιμή που υποδεικνύει αν το ProjectExternallyEdited είναι ορισμένο ή όχι. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Λαμβάνει μια τιμή που υποδεικνύει αν το RemoveFileProperties είναι ορισμένο ή όχι. |
| [get_ResourceAssignments](./get_resourceassignments/) | Λαμβάνει το αντικείμενο ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Λαμβάνει όλους τους ορισμούς φίλτρων που βασίζονται σε πόρους. ResourceFilters είναι μια συλλογή αντικειμένων Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Λαμβάνει όλους τους ορισμούς ομάδων που βασίζονται σε πόρους. ResourceGroups είναι μια συλλογή αντικειμένων Group. |
| [get_Resources](./get_resources/) | Λαμβάνει το αντικείμενο ResourceCollection. |
| [get_Revision](./get_revision/) | Λαμβάνει μια τιμή του Revision. |
| [get_RootTask](./get_roottask/) | Λαμβάνει τη ρίζα του δέντρου των εργασιών. |
| [get_SaveVersion](./get_saveversion/) | Λαμβάνει μια τιμή του SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ScheduleFromStart είναι ορισμένο ή όχι. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ShowProjectSummaryTask είναι ορισμένο ή όχι. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το SplitsInProgressTasks είναι ορισμένο ή όχι. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το SpreadActualCost είναι ορισμένο ή όχι. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το SpreadPercentComplete είναι ορισμένο ή όχι. |
| [get_StartDate](./get_startdate/) | Λαμβάνει μια τιμή του StartDate. |
| [get_StatusDate](./get_statusdate/) | Λαμβάνει μια τιμή του StatusDate. |
| [get_Subject](./get_subject/) | Λαμβάνει μια τιμή του Subject. |
| [get_Tables](./get_tables/) | Λαμβάνει μια λίστα αντικειμένων Table. |
| [get_TaskFilters](./get_taskfilters/) | Λαμβάνει όλους τους ορισμούς φίλτρων που βασίζονται σε εργασίες. TaskFilters είναι μια συλλογή αντικειμένων Filter. |
| [get_TaskGroups](./get_taskgroups/) | Λαμβάνει όλους τους ορισμούς ομάδων που βασίζονται σε εργασίες. TaskGroups είναι μια συλλογή αντικειμένων Group. |
| [get_TaskLinks](./get_tasklinks/) | Λαμβάνει το αντικείμενο TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το TaskUpdatesResource είναι ορισμένο ή όχι. |
| [get_Template](./get_template/) | Λαμβάνει μια τιμή του Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Λαμβάνει μια τιμή του TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Λαμβάνει μια τιμή του TimescaleStart. |
| [get_Title](./get_title/) | Λαμβάνει μια τιμή του Title. |
| [get_Uid](./get_uid/) | Λαμβάνει μια τιμή του Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το UpdateManuallyScheduledTasksWhenEditingLinks είναι ορισμένο ή όχι. |
| [get_VbaProject](./get_vbaproject/) | Λαμβάνει μια παρουσία της κλάσης VbaProject. |
| [get_Views](./get_views/) | Λαμβάνει μια λίστα αντικειμένων View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Λαμβάνει τον ορισμό WBS Code Definition για το έργο. |
| [get_WeekStartDay](./get_weekstartday/) | Λαμβάνει μια τιμή του WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Λαμβάνει μια τιμή του WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Επιστρέφει το χρόνο αποθήκευσης του baseline. |
| [GetDuration (3 overloads)](./getduration/) | Λαμβάνει αντικείμενο Duration με τον καθορισμένο αριθμό μονάδων και την προεπιλεγμένη μορφή διάρκειας που ορίζεται στις ρυθμίσεις του έργου Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλεγμένη Timescale (Days). |
| [GetPredecessors](./getpredecessors/) | Επιστρέφει μια συλλογή task links που είναι προκάτοχοι της καθορισμένης εργασίας. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Λαμβάνει πληροφορίες αρχείου έργου από το stream. |
| [GetWork](./getwork/) | Λαμβάνει αντικείμενο Duration με την καθορισμένη τιμή double και την προεπιλεγμένη work format. |
| [Recalculate (2 overloads)](./recalculate/) | Αναπρογραμματίζει όλα τα ids εργασιών του έργου, τα επίπεδα περιγράμματος, τις ημερομηνίες έναρξης/λήξης, ορίζει τις πρώιμες/τελευταίες ημερομηνίες, υπολογίζει τα slacks, work και cost fields. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Επαναϋπολογίζει το Id, την Start και το Finish των resources. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Επαναϋπολογίζει την Start και το Finish των resources. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Αφαιρεί μη έγκυρες resource assignments από τη λίστα resource assignments του έργου. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Αναριθμεί τον κώδικα WBS όλων των εργασιών. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Αναπρογραμματίζει την ατελή εργασία του έργου ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία. |
| [Save (5 overloads)](./save/) | Αποθηκεύει το έργο σε ένα stream χρησιμοποιώντας τις καθορισμένες save options. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Αποθηκεύει το έργο ως πρότυπο σε ένα καθορισμένο stream. |
| [SaveReport (4 overloads)](./savereport/) | Αποθηκεύει την αναφορά overview report του έργου στο stream. |
| [SelectAllChildTasks](./selectallchildtasks/) | Συλλέγει αναδρομικά όλες τις child tasks της root task. |
| [Set (2 overloads)](./set/) | Αντιστοιχεί την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [set_ActualsInSync](./set_actualsinsync/) | Ορίζει μια τιμή που υποδεικνύει αν το ActualsInSync είναι ορισμένο ή όχι. |
| [set_AdminProject](./set_adminproject/) | Ορίζει μια τιμή που υποδεικνύει αν το AdminProject είναι ορισμένο ή όχι. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Ορίζει μια τιμή που υποδεικνύει αν το AreEditableActualCosts είναι ορισμένο ή όχι. |
| [set_Author](./set_author/) | Ορίζει μια τιμή του Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Ορίζει μια τιμή που υποδεικνύει αν το AutoAddNewResourcesAndTasks είναι ορισμένο ή όχι. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Ορίζει εάν το κόστος ανάθεσης και το εναπομείναν κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία της ανάθεσης και τους ρυθμούς των πόρων. |
| [set_Autolink](./set_autolink/) | Ορίζει μια τιμή που υποδεικνύει εάν το Autolink είναι ενεργοποιημένο ή όχι. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Ορίζει μια τιμή του BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Ορίζει τη λειτουργία υπολογισμού ενός έργου. Μπορεί να είναι μία από τις τιμές της απαρίθμησης CalculationMode. |
| [set_Calendar](./set_calendar/) | Ορίζει μια τιμή του Calendar. |
| [set_Category](./set_category/) | Ορίζει μια τιμή της Category. |
| [set_Comments](./set_comments/) | Ορίζει μια τιμή των Comments. |
| [set_Company](./set_company/) | Ορίζει μια τιμή της Company. |
| [set_CreationDate](./set_creationdate/) | Ορίζει μια τιμή του CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Ορίζει μια τιμή του CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Ορίζει μια τιμή του CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Ορίζει μια τιμή του CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Ορίζει μια τιμή του CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Ορίζει μια τιμή του CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Ορίζει μια τιμή του CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Ορίζει μια τιμή του CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Ορίζει μια τιμή του DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Ορίζει μια τιμή του DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Ορίζει μια τιμή του DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Ορίζει μια τιμή του DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Ορίζει μια τιμή του DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Ορίζει μια τιμή του DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Ορίζει μια τιμή του DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Ορίζει μια τιμή του DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Ορίζει μια τιμή του DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Ορίζει την προεπιλεγμένη προβολή του έργου. |
| [set_DurationFormat](./set_durationformat/) | Ορίζει μια τιμή του DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Ορίζει μια τιμή του EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Ορίζει μια τιμή του ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Ορίζει μια τιμή του FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Ορίζει μια τιμή που υποδεικνύει αν το FiscalYearStart είναι ορισμένο ή όχι. |
| [set_FyStartDate](./set_fystartdate/) | Ορίζει μια τιμή του FyStartDate. |
| [set_Guid](./set_guid/) | Ορίζει μια τιμή του Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Ορίζει μια τιμή που υποδεικνύει αν το HonorConstraints είναι ορισμένο ή όχι. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Ορίζει μια τιμή του HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Ορίζει μια τιμή που υποδεικνύει αν το InsertedProjectsLikeSummary είναι ορισμένο ή όχι. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Ορίζει μια τιμή που υποδεικνύει αν το KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled είναι ορισμένο ή όχι. |
| [set_Keywords](./set_keywords/) | Ορίζει μια τιμή του Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Ορίζει μια τιμή του LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Ορίζει μια τιμή του LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Ορίζει μια τιμή του LastSaved. |
| [set_Manager](./set_manager/) | Ορίζει μια τιμή του Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Ορίζει μια τιμή που υποδεικνύει αν το MicrosoftProjectServerURL είναι ορισμένο ή όχι. |
| [set_MinutesPerDay](./set_minutesperday/) | Ορίζει μια τιμή του MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Ορίζει μια τιμή του MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Ορίζει μια τιμή που υποδεικνύει αν το MoveCompletedEndsBack είναι ορισμένο ή όχι. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Ορίζει μια τιμή που υποδεικνύει αν το MoveCompletedEndsForward είναι ορισμένο ή όχι. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Ορίζει μια τιμή που υποδεικνύει αν το MoveRemainingStartsBack είναι ορισμένο ή όχι. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Ορίζει μια τιμή που υποδεικνύει αν το MoveRemainingStartsForward είναι ορισμένο ή όχι. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Ορίζει μια τιμή που υποδεικνύει αν το MultipleCriticalPaths είναι ορισμένο ή όχι. |
| [set_Name](./set_name/) | Ορίζει μια τιμή του Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Ορίζει μια τιμή που υποδεικνύει αν το NewTasksAreManual είναι ορισμένο ή όχι. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Ορίζει μια τιμή που υποδεικνύει αν το NewTasksEffortDriven είναι ορισμένο ή όχι. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Ορίζει μια τιμή που υποδεικνύει εάν το NewTasksEstimated είναι ορισμένο ή όχι. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Ορίζει μια τιμή του NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Ορίζει μια τιμή που υποδεικνύει εάν το ProjectExternallyEdited είναι ορισμένο ή όχι. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Ορίζει μια τιμή που υποδεικνύει εάν το RemoveFileProperties είναι ορισμένο ή όχι. |
| [set_Revision](./set_revision/) | Ορίζει μια τιμή του Revision. |
| [set_SaveVersion](./set_saveversion/) | Ορίζει μια τιμή του SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Ορίζει μια τιμή που υποδεικνύει εάν το ScheduleFromStart είναι ορισμένο ή όχι. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Ορίζει μια τιμή που υποδεικνύει εάν το ShowProjectSummaryTask είναι ορισμένο ή όχι. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Ορίζει μια τιμή που υποδεικνύει εάν το SplitsInProgressTasks είναι ορισμένο ή όχι. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Ορίζει μια τιμή που υποδεικνύει εάν το SpreadActualCost είναι ορισμένο ή όχι. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Ορίζει μια τιμή που υποδεικνύει εάν το SpreadPercentComplete είναι ορισμένο ή όχι. |
| [set_StartDate](./set_startdate/) | Ορίζει μια τιμή του StartDate. |
| [set_StatusDate](./set_statusdate/) | Ορίζει μια τιμή του StatusDate. |
| [set_Subject](./set_subject/) | Ορίζει μια τιμή του Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Ορίζει μια τιμή που υποδεικνύει εάν το TaskUpdatesResource είναι ορισμένο ή όχι. |
| [set_Template](./set_template/) | Ορίζει μια τιμή του Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Ορίζει μια τιμή του TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Ορίζει μια τιμή του TimescaleStart. |
| [set_Title](./set_title/) | Ορίζει μια τιμή του Title. |
| [set_Uid](./set_uid/) | Ορίζει μια τιμή του Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Ορίζει μια τιμή που υποδεικνύει εάν το UpdateManuallyScheduledTasksWhenEditingLinks είναι ορισμένο ή όχι. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Ορίζει τον ορισμό κώδικα WBS για το έργο. |
| [set_WeekStartDay](./set_weekstartday/) | Ορίζει μια τιμή του WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Ορίζει μια τιμή του WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Αποθηκεύει τα πεδία βάσης στην καθορισμένη βάση για ολόκληρο το έργο. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Ορίζει το χρόνο αποθήκευσης της βάσης. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Ενημερώνει όλη τη δουλειά ως ολοκληρωμένη μέσω μιας καθορισμένης ημερομηνίας για ολόκληρο το έργο. |

