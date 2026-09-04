---
title: "Resource"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά έναν πόρο σε ένα έργο."
type: docs
weight: 248
url: /el/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Αναπαριστά έναν πόρο σε ένα έργο.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [canLevel()](#canLevel--) | Λαμβάνει μια τιμή που υποδεικνύει αν το CanLevel είναι ορισμένο ή όχι. |
| [delete()](#delete--) | Διαγράφει έναν πόρο και τις αναθέσεις του από το έργο. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getACWP()](#getACWP--) | Λαμβάνει μια τιμή του ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Λαμβάνει μια τιμή του AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Λαμβάνει μια τιμή του ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Λαμβάνει μια τιμή του ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Λαμβάνει μια τιμή του ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Λαμβάνει μια τιμή του ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Λαμβάνει μια τιμή του ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Λαμβάνει μια τιμή του ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Λαμβάνει μια τιμή του ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Λαμβάνει μια τιμή του AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Λαμβάνει μια τιμή του AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Λαμβάνει μια συλλογή αναθέσεων πόρων για αυτό το αντικείμενο. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Λαμβάνει την παρουσία της κλάσης [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Λαμβάνει μια τιμή του AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Λαμβάνει μια τιμή του AvailableTo. |
| [getBCWP()](#getBCWP--) | Λαμβάνει μια τιμή του BCWP. |
| [getBCWS()](#getBCWS--) | Λαμβάνει μια τιμή του BCWS. |
| [getBaselines()](#getBaselines--) | Λαμβάνει μια παρουσία του BaselineCollection για αυτό το αντικείμενο. |
| [getBookingType()](#getBookingType--) | Λαμβάνει μια τιμή του BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Λαμβάνει μια τιμή του BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Λαμβάνει μια τιμή του BudgetWork. |
| [getCV()](#getCV--) | Λαμβάνει μια τιμή του CV. |
| [getCalendar()](#getCalendar--) | Λαμβάνει μια τιμή του Calendar. |
| [getCode()](#getCode--) | Λαμβάνει μια τιμή του Code. |
| [getCost()](#getCost--) | Λαμβάνει μια τιμή του Cost. |
| [getCostCenter()](#getCostCenter--) | Λαμβάνει μια τιμή του CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Λαμβάνει μια τιμή του CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Λαμβάνει μια τιμή του CostVariance. |
| [getCreated()](#getCreated--) | Λαμβάνει μια τιμή του Created. |
| [getEMailAddress()](#getEMailAddress--) | Λαμβάνει μια τιμή του EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Λαμβάνει τις τιμές ενός εκτεταμένου χαρακτηριστικού. |
| [getFinish()](#getFinish--) | Λαμβάνει μια τιμή του Finish. |
| [getGroup()](#getGroup--) | Λαμβάνει μια τιμή του Group. |
| [getGuid()](#getGuid--) | Λαμβάνει μια τιμή του Guid. |
| [getHyperlink()](#getHyperlink--) | Λαμβάνει τον τίτλο ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Λαμβάνει τη διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Λαμβάνει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο. |
| [getId()](#getId--) | Λαμβάνει μια τιμή του Id. |
| [getInactive()](#getInactive--) | Λαμβάνει μια τιμή που υποδεικνύει αν το Inactive είναι ορισμένο ή όχι. |
| [getInitials()](#getInitials--) | Λαμβάνει μια τιμή του Initials. |
| [getItems()](#getItems--) | Λαμβάνει τους υπο-πόρους. |
| [getMaterialLabel()](#getMaterialLabel--) | Λαμβάνει μια τιμή του MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Λαμβάνει μια τιμή του MaxUnits. |
| [getName()](#getName--) | Λαμβάνει μια τιμή του Name. |
| [getNotesRTF()](#getNotesRTF--) | Λαμβάνει μια τιμή του NotesRTF. |
| [getNotesText()](#getNotesText--) | Λαμβάνει μια τιμή του NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Λαμβάνει ένα αντικείμενο OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | Λαμβάνει μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι. |
| [getOvertimeCost()](#getOvertimeCost--) | Λαμβάνει μια τιμή του OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Λαμβάνει μια τιμή του OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Λαμβάνει μια τιμή του OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Λαμβάνει μια τιμή του OvertimeWork. |
| [getParentProject()](#getParentProject--) | Λαμβάνει το γονικό έργο για αυτό το υποδοχέα. |
| [getPeakUnits()](#getPeakUnits--) | Λαμβάνει μια τιμή του PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Λαμβάνει μια τιμή του PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Λαμβάνει μια τιμή του Phonetics. |
| [getRates()](#getRates--) | Λαμβάνει το στιγμιότυπο της κλάσης [RateCollection](../../com.aspose.tasks/ratecollection) για αυτό το αντικείμενο. |
| [getRegularWork()](#getRegularWork--) | Λαμβάνει μια τιμή του RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Λαμβάνει μια τιμή του RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Λαμβάνει μια τιμή του RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Λαμβάνει μια τιμή του RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Λαμβάνει μια τιμή του RemainingWork. |
| [getSV()](#getSV--) | Λαμβάνει μια τιμή του SV. |
| [getStandardRate()](#getStandardRate--) | Λαμβάνει μια τιμή του StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Λαμβάνει μια τιμή του StandardRateFormat. |
| [getStart()](#getStart--) | Λαμβάνει μια τιμή του Start. |
| [getTimephasedData()](#getTimephasedData--) | Λαμβάνει ένα στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Επιστρέφει [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο με `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) τιμές εντός των δοσμένων ημερομηνιών έναρξης και λήξης. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Επιστρέφει ένα στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο με το `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) τιμές εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Λαμβάνει μια τιμή του Type. |
| [getUid()](#getUid--) | Λαμβάνει μια τιμή του Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Λαμβάνει μια τιμή του WindowsUserAccount. |
| [getWork()](#getWork--) | Λαμβάνει μια τιμή του Work. |
| [getWorkVariance()](#getWorkVariance--) | Λαμβάνει μια τιμή του WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Λαμβάνει μια τιμή του Workgroup. |
| [hasChildren()](#hasChildren--) | \\{@inheritDoc\\} |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsBudget είναι ορισμένο ή όχι. |
| [isCostResource()](#isCostResource--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsCostResource είναι ορισμένο ή όχι. |
| [isEnterprise()](#isEnterprise--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsEnterprise είναι ορισμένο ή όχι. |
| [isGeneric()](#isGeneric--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsGeneric είναι ορισμένο ή όχι. |
| [isNull()](#isNull--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsNull είναι ορισμένο ή όχι. |
| [isRoot()](#isRoot--) | Λαμβάνει τη σημαία που υποδεικνύει αν ο πόρος είναι ριζικός πόρος. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Λαμβάνει μια τιμή που υποδεικνύει αν το IsTeamAssignmentPool είναι ορισμένο ή όχι. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [setACWP(double value)](#setACWP-double-) | Ορίζει μια τιμή του ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Ορίζει μια τιμή του AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Ορίζει μια τιμή του ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Ορίζει μια τιμή του ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Ορίζει μια τιμή του AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Ορίζει μια τιμή του AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Ορίζει μια τιμή του AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Ορίζει μια τιμή του AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Ορίζει μια τιμή του BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Ορίζει μια τιμή του BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Ορίζει μια τιμή για το BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το IsBudget είναι ορισμένο ή όχι. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Ορίζει μια τιμή για το BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή για το BudgetWork. |
| [setCV(double value)](#setCV-double-) | Ορίζει μια τιμή για το CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Ορίζει μια τιμή για το Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το CanLevel είναι ορισμένο ή όχι. |
| [setCode(String value)](#setCode-java.lang.String-) | Ορίζει μια τιμή για το Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Ορίζει μια τιμή για το Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Ορίζει μια τιμή για το CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Ορίζει μια τιμή για το CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το IsCostResource είναι ορισμένο ή όχι. |
| [setCostVariance(double value)](#setCostVariance-double-) | Ορίζει μια τιμή για το CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Ορίζει μια τιμή για το Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Ορίζει μια τιμή για το EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το IsEnterprise είναι ορισμένο ή όχι. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ορίζει μια τιμή για το Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το IsGeneric είναι ορισμένο ή όχι. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Ορίζει μια τιμή για το Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Ορίζει μια τιμή για το Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Ορίζει τον τίτλο ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Ορίζει τη διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Ορίζει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο. |
| [setId(int value)](#setId-int-) | Ορίζει μια τιμή για το Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει αν το Inactive είναι ορισμένο ή όχι. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Ορίζει μια τιμή του Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Ορίζει μια τιμή του MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Ορίζει μια τιμή του MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει μια τιμή του Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Ορίζει μια τιμή του NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Ορίζει μια τιμή του NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το IsNull είναι ορισμένο ή όχι. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Ορίζει μια τιμή που υποδεικνύει εάν το Overallocated είναι ορισμένο ή όχι. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Ορίζει μια τιμή του OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Ορίζει μια τιμή του OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Ορίζει μια τιμή του PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Ορίζει μια τιμή του PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Ορίζει μια τιμή του Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Ορίζει μια τιμή του RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RemainingWork. |
| [setSV(double value)](#setSV-double-) | Ορίζει μια τιμή του SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Ορίζει μια τιμή του StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Ορίζει μια τιμή του StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ορίζει μια τιμή του Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το IsTeamAssignmentPool είναι ορισμένο ή όχι. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ορίζει μια παρουσία της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο. |
| [setType(int value)](#setType-int-) | Ορίζει μια τιμή του Type. |
| [setUid(int value)](#setUid-int-) | Ορίζει μια τιμή του Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Ορίζει μια τιμή του WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Ορίζει μια τιμή του WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Ορίζει μια τιμή του Workgroup. |
| [toString()](#toString--) | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Rsc](../../com.aspose.tasks/rsc) για λήψη του κλειδιού ιδιότητας. |

**Returns:**
T - η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Rsc](../../com.aspose.tasks/rsc) για λήψη του κλειδιού ιδιότητας. |
| val | T | η τιμή. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το CanLevel είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Διαγράφει έναν πόρο και τις αναθέσεις του από το έργο.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | Η καθορισμένη παρουσία της κλάσης [Resource](../../com.aspose.tasks/resource) για σύγκριση με αυτήν την παρουσία. |

**Returns:**
boolean - **True** εάν η καθορισμένη παρουσία της κλάσης [Resource](../../com.aspose.tasks/resource) έχει την ίδια τιμή Uid με αυτήν την παρουσία· διαφορετικά, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

**Returns:**
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα Resource που έχει την ίδια τιμή Uid με αυτήν την παρουσία· διαφορετικά, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Λαμβάνει μια τιμή του ACWP.

**Returns:**
double - μια τιμή του ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Λαμβάνει μια τιμή του AccrueAt.

**Returns:**
int - μια τιμή του AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Λαμβάνει μια τιμή του ActiveDirectoryGuid.

**Returns:**
java.lang.String - μια τιμή του ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Λαμβάνει μια τιμή του ActualCost.

**Returns:**
java.math.BigDecimal - μια τιμή του ActualCost.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Λαμβάνει μια τιμή του ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - μια τιμή του ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Λαμβάνει μια τιμή του ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Λαμβάνει μια τιμή του ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Λαμβάνει μια τιμή του ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Λαμβάνει μια τιμή του ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Λαμβάνει μια τιμή του AssignmentOwner.

**Returns:**
java.lang.String - μια τιμή του AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Λαμβάνει μια τιμή του AssignmentOwnerGuid.

**Returns:**
java.lang.String - μια τιμή του AssignmentOwnerGuid.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Λαμβάνει μια συλλογή αναθέσεων πόρων για αυτό το αντικείμενο.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Λαμβάνει την παρουσία της κλάσης [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). Η συλλογή των περιόδων κατά τις οποίες ένας πόρος είναι διαθέσιμος.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Λαμβάνει μια τιμή του AvailableFrom.

**Returns:**
java.util.Date - μια τιμή του AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Λαμβάνει μια τιμή του AvailableTo.

**Returns:**
java.util.Date - μια τιμή του AvailableTo.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Λαμβάνει μια τιμή του BCWP.

**Returns:**
double - μια τιμή του BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Λαμβάνει μια τιμή του BCWS.

**Returns:**
double - μια τιμή του BCWS.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Λαμβάνει ένα αντικείμενο BaselineCollection για αυτό το αντικείμενο. Οι τιμές βάσης για έναν πόρο.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Λαμβάνει μια τιμή του BookingType.

**Returns:**
int - μια τιμή του BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Λαμβάνει μια τιμή του BudgetCost.

**Returns:**
java.math.BigDecimal - μια τιμή του BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Λαμβάνει μια τιμή του BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Λαμβάνει μια τιμή του CV.

**Returns:**
double - μια τιμή του CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Λαμβάνει μια τιμή του Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Λαμβάνει μια τιμή του Code.

**Returns:**
java.lang.String - μια τιμή του Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Λαμβάνει μια τιμή του Cost.

**Returns:**
java.math.BigDecimal - μια τιμή του Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Λαμβάνει μια τιμή του CostCenter.

**Returns:**
java.lang.String - μια τιμή του CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Λαμβάνει μια τιμή του CostPerUse.

**Returns:**
java.math.BigDecimal - μια τιμή του CostPerUse.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Λαμβάνει μια τιμή του CostVariance.

**Returns:**
double - μια τιμή του CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Λαμβάνει μια τιμή του Created.

**Returns:**
java.util.Date - μια τιμή του Created.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Λαμβάνει μια τιμή του EMailAddress.

**Returns:**
java.lang.String - μια τιμή του EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Λαμβάνει τις τιμές ενός εκτεταμένου χαρακτηριστικού.

--------------------

Απαιτούνται δύο κομμάτια δεδομένων - ένας δείκτης πίσω στον πίνακα επεκταμένων χαρακτηριστικών που καθορίζεται είτε από το μοναδικό ID είτε από το Field ID, και η τιμή που καθορίζεται είτε με την τιμή, είτε με έναν δείκτη πίσω στη λίστα τιμών.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Λαμβάνει μια τιμή του Finish.

**Returns:**
java.util.Date - μια τιμή του Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Λαμβάνει μια τιμή του Group.

**Returns:**
java.lang.String - μια τιμή του Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Λαμβάνει μια τιμή του Guid.

**Returns:**
java.lang.String - μια τιμή του Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Λαμβάνει τον τίτλο ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

**Returns:**
java.lang.String - ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Λαμβάνει τη διεύθυνση ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

**Returns:**
java.lang.String - η διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Λαμβάνει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

**Returns:**
java.lang.String - η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο.
### getId() {#getId--}
```
public final int getId()
```


Λαμβάνει μια τιμή του Id.

**Returns:**
int - μια τιμή του Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το Inactive είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Λαμβάνει μια τιμή του Initials.

**Returns:**
java.lang.String - μια τιμή του Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Λαμβάνει τους υπο-πόρους.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - παιδικοί πόροι.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Λαμβάνει μια τιμή του MaterialLabel.

**Returns:**
java.lang.String - μια τιμή του MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Λαμβάνει μια τιμή του MaxUnits.

**Returns:**
double - μια τιμή του MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει μια τιμή του Name.

**Returns:**
java.lang.String - μια τιμή του Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Λαμβάνει μια τιμή του NotesRTF.

**Returns:**
java.lang.String - μια τιμή του NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Λαμβάνει μια τιμή του NotesText.

**Returns:**
java.lang.String - μια τιμή του NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Λαμβάνει ένα αντικείμενο OutlineCodeCollection. Η τιμή ενός κώδικα περιγράμματος.

--------------------

Απαιτούνται δύο κομμάτια δεδομένων - ένας δείκτης στον πίνακα κώδικα περιγράμματος που καθορίζεται από το FieldID, και η τιμή που καθορίζεται είτε από το ValueID είτε από το ValueGUID δείκτη στη λίστα τιμών.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Λαμβάνει μια τιμή του OvertimeCost.

**Returns:**
java.math.BigDecimal - μια τιμή του OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Λαμβάνει μια τιμή του OvertimeRate.

**Returns:**
java.math.BigDecimal - μια τιμή του OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Λαμβάνει μια τιμή του OvertimeRateFormat.

**Returns:**
int - μια τιμή του OvertimeRateFormat.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Λαμβάνει μια τιμή του OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Λαμβάνει το γονικό έργο για αυτό το υποδοχέα.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Λαμβάνει μια τιμή του PeakUnits.

**Returns:**
double - μια τιμή του PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Λαμβάνει μια τιμή του PercentWorkComplete.

**Returns:**
int - μια τιμή του PercentWorkComplete.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Λαμβάνει μια τιμή του Phonetics.

**Returns:**
java.lang.String - μια τιμή του Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Λαμβάνει το στιγμιότυπο της κλάσης [RateCollection](../../com.aspose.tasks/ratecollection) για αυτό το αντικείμενο. Η συλλογή περιόδων και τιμών που σχετίζονται με κάθε μία.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Λαμβάνει μια τιμή του RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Λαμβάνει μια τιμή του RemainingCost.

**Returns:**
java.math.BigDecimal - μια τιμή του RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Λαμβάνει μια τιμή του RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - μια τιμή του RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Λαμβάνει μια τιμή του RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Λαμβάνει μια τιμή του RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


Λαμβάνει μια τιμή του SV.

**Returns:**
double - μια τιμή του SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Λαμβάνει μια τιμή του StandardRate.

**Returns:**
java.math.BigDecimal - μια τιμή του StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Λαμβάνει μια τιμή του StandardRateFormat.

**Returns:**
int - μια τιμή του StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Λαμβάνει μια τιμή του Start.

**Returns:**
java.util.Date - μια τιμή του Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Λαμβάνει ένα στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο.

--------------------

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Επιστρέφει [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο με `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) τιμές εντός των δοσμένων ημερομηνιών έναρξης και λήξης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| τέλος | java.util.Date | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Επιστρέφει ένα στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο με το `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) τιμές εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| τέλος | java.util.Date | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |
| timephasedType | byte | Ο τύπος των δεδομένων χρονικής φάσης ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Λαμβάνει μια τιμή του Type.

**Returns:**
int - μια τιμή του Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Λαμβάνει μια τιμή του Uid.

**Returns:**
int - μια τιμή του Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Λαμβάνει μια τιμή του WindowsUserAccount.

**Returns:**
java.lang.String - μια τιμή του WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Λαμβάνει μια τιμή του Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Λαμβάνει μια τιμή του WorkVariance.

**Returns:**
double - μια τιμή του WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Λαμβάνει μια τιμή του Workgroup.

**Returns:**
int - μια τιμή του Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Δεσμευμένο για εσωτερική χρήση.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsBudget είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsCostResource είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsEnterprise είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsGeneric είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsNull είναι ορισμένο ή όχι.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Αποκτά τη σημαία που υποδεικνύει εάν ο πόρος είναι ριζικός πόρος. Ο ριζικός πόρος είναι ένας ειδικός πόρος που προορίζεται να υποστηρίζει τις εσωτερικές λειτουργίες των μορφών του MS Project και δεν προορίζεται να χρησιμοποιείται άμεσα από τον κώδικα του χρήστη.

**Returns:**
boolean - η σημαία που υποδεικνύει εάν ο πόρος είναι ριζικός πόρος.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το IsTeamAssignmentPool είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το IsTeamAssignmentPool είναι ορισμένο ή όχι.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Rsc](../../com.aspose.tasks/rsc) για λήψη του κλειδιού ιδιότητας. |
| val | java.util.Date | η τιμή. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Ορίζει μια τιμή του ACWP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Ορίζει μια τιμή του AccrueAt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Ορίζει μια τιμή του ActiveDirectoryGuid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Ορίζει μια τιμή του ActualCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του ActualCost. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Ορίζει μια τιμή του ActualOvertimeCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Ορίζει μια τιμή του ActualOvertimeWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Ορίζει μια τιμή του ActualOvertimeWorkProtected.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του ActualOvertimeWorkProtected. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Ορίζει μια τιμή του ActualWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Ορίζει μια τιμή του ActualWorkProtected.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Ορίζει μια τιμή του AssignmentOwner.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Ορίζει μια τιμή του AssignmentOwnerGuid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του AssignmentOwnerGuid. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Ορίζει μια τιμή του AvailableFrom.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Ορίζει μια τιμή του AvailableTo.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του AvailableTo. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Ορίζει μια τιμή του BCWP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Ορίζει μια τιμή του BCWS.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Ορίζει μια τιμή για το BookingType.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του BookingType. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το IsBudget είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει εάν το IsBudget είναι ορισμένο ή όχι. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Ορίζει μια τιμή για το BudgetCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Ορίζει μια τιμή για το BudgetWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Ορίζει μια τιμή για το CV.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Ορίζει μια τιμή για το Calendar.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | μια τιμή του Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το CanLevel είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει εάν το CanLevel είναι ορισμένο ή όχι. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Ορίζει μια τιμή για το Code.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Ορίζει μια τιμή για το Cost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Ορίζει μια τιμή για το CostCenter.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Ορίζει μια τιμή για το CostPerUse.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το IsCostResource είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει εάν το IsCostResource είναι ορισμένο ή όχι. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Ορίζει μια τιμή για το CostVariance.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Ορίζει μια τιμή για το Created.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Created. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Ορίζει μια τιμή για το EMailAddress.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το IsEnterprise είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει εάν το IsEnterprise είναι ορισμένο ή όχι. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ορίζει μια τιμή για το Finish.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το IsGeneric είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει εάν το IsGeneric είναι ορισμένο ή όχι. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Ορίζει μια τιμή για το Group.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Ορίζει μια τιμή για το Guid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Ορίζει τον τίτλο ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ο τίτλος ή το επεξηγηματικό κείμενο ενός υπερσυνδέσμου που σχετίζεται με έναν πόρο. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Ορίζει τη διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η διεύθυνση για έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Ορίζει τη συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο.

--------------------

Η πλήρης διεύθυνση (Hyperlink Href στο Microsoft Project) του υπερσυνδέσμου είναι μια συνένωση του HyperlinkAddress και του HyperlinkSubAddress.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η συγκεκριμένη θέση σε ένα έγγραφο σε έναν υπερσύνδεσμο που σχετίζεται με έναν πόρο. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Ορίζει μια τιμή για το Id.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει αν το Inactive είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει αν το Inactive είναι ορισμένο ή όχι. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Ορίζει μια τιμή του Initials.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Ορίζει μια τιμή του MaterialLabel.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Ορίζει μια τιμή του MaxUnits.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ορίζει μια τιμή του Name.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Ορίζει μια τιμή του NotesRTF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Ορίζει μια τιμή του NotesText.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το IsNull είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει αν το IsNull είναι ορισμένο ή όχι. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Overallocated είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Ορίζει μια τιμή του OvertimeCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Ορίζει μια τιμή του OvertimeRate.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Ορίζει μια τιμή του OvertimeRateFormat.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του OvertimeRateFormat. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Ορίζει μια τιμή του OvertimeWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Ορίζει μια τιμή του PeakUnits.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Ορίζει μια τιμή του PercentWorkComplete.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του PercentWorkComplete. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Ορίζει μια τιμή του Phonetics.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Phonetics. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Ορίζει μια τιμή του RegularWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Ορίζει μια τιμή του RemainingCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Ορίζει μια τιμή του RemainingOvertimeCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Ορίζει μια τιμή του RemainingOvertimeWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Ορίζει μια τιμή του RemainingWork.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του RemainingWork. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Ορίζει μια τιμή του SV.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Ορίζει μια τιμή του StandardRate.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Ορίζει μια τιμή του StandardRateFormat.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ορίζει μια τιμή του Start.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το IsTeamAssignmentPool είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το IsTeamAssignmentPool είναι ορισμένο ή όχι. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ορίζει μια παρουσία της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο.

--------------------

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | ένα στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) για αυτό το αντικείμενο. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Ορίζει μια τιμή του Type.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ορίζει μια τιμή του Uid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Ορίζει μια τιμή του WindowsUserAccount.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ορίζει μια τιμή του Work.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Ορίζει μια τιμή του WorkVariance.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Ορίζει μια τιμή του Workgroup.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει σύντομη αναπαράσταση σε συμβολοσειρά του στιγμιότυπου της κλάσης [Resource](../../com.aspose.tasks/resource). Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

**Returns:**
java.lang.String - σύντομη συμβολοσειρά που αντιπροσωπεύει το αντικείμενο πόρου.
