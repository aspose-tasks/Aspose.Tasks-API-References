---
title: "ResourceAssignment"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια ανάθεση πόρου σε ένα έργο."
type: docs
weight: 249
url: /el/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Αναπαριστά μια ανάθεση πόρου σε ένα έργο.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο. |
| [delete()](#delete--) | Διαγράφει την ανάθεση πόρων από τη συλλογή αναθέσεων του έργου. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getACWP()](#getACWP--) | Λαμβάνει μια τιμή του ACWP. |
| [getActualCost()](#getActualCost--) | Λαμβάνει μια τιμή του ActualCost. |
| [getActualFinish()](#getActualFinish--) | Λαμβάνει μια τιμή του ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Λαμβάνει μια τιμή του ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Λαμβάνει μια τιμή του ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Λαμβάνει μια τιμή του ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Λαμβάνει μια τιμή του ActualStart. |
| [getActualWork()](#getActualWork--) | Λαμβάνει μια τιμή του ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Λαμβάνει μια τιμή του ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Λαμβάνει μια τιμή του AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Λαμβάνει μια τιμή του AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Λαμβάνει μια τιμή του BCWP. |
| [getBCWS()](#getBCWS--) | Λαμβάνει μια τιμή του BCWS. |
| [getBaselines()](#getBaselines--) | Λαμβάνει το αντικείμενο AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | Λαμβάνει μια τιμή του BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Λαμβάνει μια τιμή του BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Λαμβάνει μια τιμή του BudgetWork. |
| [getCV()](#getCV--) | Λαμβάνει μια τιμή του CV. |
| [getConfirmed()](#getConfirmed--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το Confirmed έχει οριστεί ή όχι. |
| [getCost()](#getCost--) | Λαμβάνει μια τιμή του Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Λαμβάνει μια τιμή του CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Λαμβάνει μια τιμή του CostVariance. |
| [getCreated()](#getCreated--) | Λαμβάνει μια τιμή του Created. |
| [getDelay()](#getDelay--) | Λαμβάνει μια τιμή του Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Λαμβάνει μια παρουσία της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο. |
| [getFinish()](#getFinish--) | Λαμβάνει μια τιμή του Finish. |
| [getFinishVariance()](#getFinishVariance--) | Λαμβάνει μια τιμή του FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το FixedMaterial είναι ορισμένο ή όχι. |
| [getGuid()](#getGuid--) | Λαμβάνει το μοναδικό αναγνωριστικό για αυτήν την ανάθεση. |
| [getHyperlink()](#getHyperlink--) | Λαμβάνει μια τιμή του Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Λαμβάνει μια τιμή του HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Λαμβάνει μια τιμή του HyperlinkSubAddress. |
| [getItems()](#getItems--) | \\{@inheritDoc\\} |
| [getLevelingDelay()](#getLevelingDelay--) | Λαμβάνει μια τιμή του LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το LinkedFields είναι ορισμένο ή όχι. |
| [getMilestone()](#getMilestone--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το Milestone είναι ορισμένο ή όχι. |
| [getNotesRTF()](#getNotesRTF--) | Λαμβάνει τις σημειώσεις κειμένου σε μορφή RTF. |
| [getNotesText()](#getNotesText--) | Λαμβάνει το απλό κείμενο των σημειώσεων που εξάγεται από τα δεδομένα RTF. |
| [getOverallocated()](#getOverallocated--) | Λαμβάνει μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι. |
| [getOvertimeCost()](#getOvertimeCost--) | Λαμβάνει μια τιμή του OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Λαμβάνει μια τιμή του OvertimeWork. |
| [getParentProject()](#getParentProject--) | Λαμβάνει το γονικό έργο για αυτήν την ανάθεση. |
| [getPeakUnits()](#getPeakUnits--) | Λαμβάνει μια τιμή του PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Λαμβάνει μια τιμή του PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Λαμβάνει μια τιμή του RateScale. |
| [getRegularWork()](#getRegularWork--) | Λαμβάνει μια τιμή του RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Λαμβάνει μια τιμή του RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Λαμβάνει μια τιμή του RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Λαμβάνει μια τιμή του RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Λαμβάνει μια τιμή του RemainingWork. |
| [getResource()](#getResource--) | Ο πόρος που έχει ανατεθεί σε μια εργασία. |
| [getResponsePending()](#getResponsePending--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ResponsePending είναι ορισμένο ή όχι. |
| [getResume()](#getResume--) | Λαμβάνει μια τιμή του Resume. |
| [getSV()](#getSV--) | Λαμβάνει μια τιμή του SV. |
| [getStart()](#getStart--) | Λαμβάνει μια τιμή του Start. |
| [getStartVariance()](#getStartVariance--) | Λαμβάνει μια τιμή του StartVariance. |
| [getStop()](#getStop--) | Λαμβάνει μια τιμή του Stop. |
| [getSummary()](#getSummary--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το Summary είναι ορισμένο ή όχι. |
| [getTask()](#getTask--) | Η εργασία στην οποία έχει ανατεθεί ένας πόρος. |
| [getTimephasedData()](#getTimephasedData--) | Λαμβάνει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στοιχεία του `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) κλάσης. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Επιστρέφει το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) με τις στιγμιότυπα του `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) κλάσης εντός των δοθέντων ημερομηνιών έναρξης και λήξης του [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Επιστρέφει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στιγμιότυπα του `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) κλάσης εντός των δοθέντων ημερομηνιών έναρξης και λήξης του καθορισμένου [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Λαμβάνει το ποσό του χρονομετρικού έργου για το καθορισμένο χρονικό διάστημα. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Λαμβάνει το ποσό του χρονομετρικού έργου για το καθορισμένο χρονικό διάστημα. |
| [getUid()](#getUid--) | Λαμβάνει μια τιμή του Uid. |
| [getUnits()](#getUnits--) | Λαμβάνει μια τιμή του Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το UpdateNeeded είναι ορισμένο ή όχι. |
| [getVAC()](#getVAC--) | Λαμβάνει μια τιμή του VAC. |
| [getWork()](#getWork--) | Λαμβάνει μια τιμή του Work. |
| [getWorkContour()](#getWorkContour--) | Λαμβάνει μια τιμή του WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Λαμβάνει μια τιμή του WorkVariance. |
| [hasChildren()](#hasChildren--) | Λαμβάνει μια τιμή που υποδεικνύει ότι αυτή η ανάθεση πόρων έχει παιδιά. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Λαμβάνει μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το παράδειγμα της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Δημιουργεί μια λίστα δεδομένων χρονικής φάσης. |
| [setACWP(double value)](#setACWP-double-) | Ορίζει μια τιμή του ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Ορίζει μια τιμή του ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Ορίζει μια τιμή του ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Ορίζει μια τιμή του ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Ορίζει μια τιμή του AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Ορίζει μια τιμή του AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Ορίζει μια τιμή του BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Ορίζει μια τιμή του BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Ορίζει μια τιμή για το BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Ορίζει μια τιμή για το BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή για το BudgetWork. |
| [setCV(double value)](#setCV-double-) | Ορίζει μια τιμή για το CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το Confirmed είναι ορισμένο ή όχι. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Ορίζει μια τιμή για το Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Ορίζει μια τιμή του CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Ορίζει μια τιμή για το CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Ορίζει μια τιμή για το Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Ορίζει ένα παράδειγμα της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ορίζει μια τιμή για το Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το FixedMaterial είναι ορισμένο ή όχι. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Ορίζει μοναδικό αναγνωριστικό για αυτήν την ανάθεση. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Ορίζει μια τιμή του Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Ορίζει μια τιμή του HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Ορίζει μια τιμή του HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το LinkedFields είναι ορισμένο ή όχι. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Ορίζει μονάδες για την ανάθεση ενός υλικού πόρου με μεταβλητή κατανάλωση υλικού. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το Milestone είναι ορισμένο ή όχι. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Ορίζει τις σημειώσεις κειμένου σε μορφή RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Ορίζει το απλό κείμενο των σημειώσεων που εξάγεται από τα δεδομένα RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το Overallocated είναι ορισμένο ή όχι. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Ορίζει μια τιμή του PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Ορίζει μια τιμή του PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Ορίζει μια τιμή του RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Ορίζει μια τιμή του RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Ορίζει μια τιμή του RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | Ο πόρος που έχει ανατεθεί σε μια εργασία. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν το ResponsePending είναι ορισμένο ή όχι. |
| [setResume(Date value)](#setResume-java.util.Date-) | Ορίζει μια τιμή του Resume. |
| [setSV(double value)](#setSV-double-) | Ορίζει μια τιμή του SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ορίζει μια τιμή του Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Ορίζει μια τιμή του Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το Summary είναι ορισμένο ή όχι. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | Η εργασία στην οποία έχει ανατεθεί ένας πόρος. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ορίζει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στοιχεία του `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) κλάση. |
| [setUid(int value)](#setUid-int-) | Ορίζει μια τιμή του Uid. |
| [setUnits(double value)](#setUnits-double-) | Ορίζει μια τιμή του Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το UpdateNeeded είναι ορισμένο ή όχι. |
| [setVAC(double value)](#setVAC-double-) | Ορίζει μια τιμή του VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Ορίζει μια τιμή του WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Ορίζει μια τιμή του WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Διαιρεί την εργασία σε δύο μέρη. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Δημιουργεί λίστα δεδομένων χρονικής φάσης βάσει της διάρκειας της εργασίας και της προγραμματισμένης ημερομηνίας έναρξης. |
| [toString()](#toString--) | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς του στιγμιότυπου της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Asn](../../com.aspose.tasks/asn) για λήψη του κλειδιού ιδιότητας. |

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
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | το καθορισμένο κλειδί ιδιότητας. [Asn](../../com.aspose.tasks/asn) για λήψη του κλειδιού ιδιότητας. |
| val | T | η τιμή. |

### delete() {#delete--}
```
public final void delete()
```


Διαγράφει την ανάθεση πόρων από τη συλλογή αναθέσεων του έργου.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Το καθορισμένο στιγμιότυπο της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment) για σύγκριση με αυτό το στιγμιότυπο. |

**Returns:**
boolean - **True** εάν το καθορισμένο στιγμιότυπο της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment) έχει την ίδια τιμή UID με αυτό το στιγμιότυπο· διαφορετικά, **false**.
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
boolean - **True** εάν το o είναι ένα ResourceAssignment που αναθέτει τον ίδιο πόρο και εργασία με αυτό το στιγμιότυπο· διαφορετικά, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Λαμβάνει μια τιμή του ACWP.

**Returns:**
double - μια τιμή του ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Λαμβάνει μια τιμή του ActualCost.

**Returns:**
java.math.BigDecimal - μια τιμή του ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Λαμβάνει μια τιμή του ActualFinish.

**Returns:**
java.util.Date - μια τιμή του ActualFinish.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Λαμβάνει μια τιμή του ActualStart.

**Returns:**
java.util.Date - μια τιμή του ActualStart.
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
public final AssignmentBaselineCollection getBaselines()
```


Λαμβάνει το αντικείμενο AssignmentBaselineCollection. Η συλλογή των τιμών βάσης που σχετίζονται με μια ανάθεση.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Confirmed έχει οριστεί ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το Confirmed είναι ορισμένο ή όχι.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Λαμβάνει μια τιμή του Cost.

**Returns:**
java.math.BigDecimal - μια τιμή του Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Λαμβάνει μια τιμή του CostRateTableType.

**Returns:**
int - μια τιμή του CostRateTableType.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Λαμβάνει μια τιμή του Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Λαμβάνει μια παρουσία της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο.

--------------------

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Λαμβάνει μια τιμή του Finish.

**Returns:**
java.util.Date - μια τιμή του Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Λαμβάνει μια τιμή του FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το FixedMaterial είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το FixedMaterial είναι ορισμένο ή όχι.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Λαμβάνει το μοναδικό αναγνωριστικό για αυτήν την ανάθεση.

**Returns:**
java.util.UUID - μοναδικό αναγνωριστικό για αυτήν την ανάθεση.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Λαμβάνει μια τιμή του Hyperlink.

**Returns:**
java.lang.String - μια τιμή του Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Λαμβάνει μια τιμή του HyperlinkAddress.

**Returns:**
java.lang.String - μια τιμή του HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Λαμβάνει μια τιμή του HyperlinkSubAddress.

**Returns:**
java.lang.String - μια τιμή του HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Δεσμευμένο για εσωτερική χρήση.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Λαμβάνει μια τιμή του LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το LinkedFields είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το LinkedFields είναι ορισμένο ή όχι.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Milestone είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το Milestone είναι ορισμένο ή όχι.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Λαμβάνει τις σημειώσεις κειμένου σε μορφή RTF.

--------------------

Υποστηρίζεται μόνο για μορφές MPP.

**Returns:**
java.lang.String - το κείμενο σημειώσεων σε μορφή RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Λαμβάνει το απλό κείμενο των σημειώσεων που εξάγεται από τα δεδομένα RTF.

**Returns:**
java.lang.String - το απλό κείμενο των σημειώσεων που εξήχθη από τα δεδομένα RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Λαμβάνει μια τιμή του OvertimeCost.

**Returns:**
java.math.BigDecimal - μια τιμή του OvertimeCost.
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


Λαμβάνει το γονικό έργο για αυτήν την ανάθεση.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Λαμβάνει μια τιμή του RateScale.

**Returns:**
int - μια τιμή του RateScale.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


Ο πόρος που έχει ανατεθεί σε μια εργασία.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το ResponsePending είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το ResponsePending είναι ορισμένο ή όχι.
### getResume() {#getResume--}
```
public final Date getResume()
```


Λαμβάνει μια τιμή του Resume.

**Returns:**
java.util.Date - μια τιμή του Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Λαμβάνει μια τιμή του SV.

**Returns:**
double - μια τιμή του SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Λαμβάνει μια τιμή του Start.

**Returns:**
java.util.Date - μια τιμή του Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Λαμβάνει μια τιμή του StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Λαμβάνει μια τιμή του Stop.

**Returns:**
java.util.Date - μια τιμή του Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Summary είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το Summary είναι ορισμένο ή όχι.
### getTask() {#getTask--}
```
public final Task getTask()
```


Η εργασία στην οποία έχει ανατεθεί ένας πόρος.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Λαμβάνει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στοιχεία του `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) κλάσης.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Επιστρέφει το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) με τις στιγμιότυπα του `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) κλάσης εντός των δοθέντων ημερομηνιών έναρξης και λήξης του [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| τέλος | java.util.Date | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Επιστρέφει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στιγμιότυπα του `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) κλάσης εντός των δοθέντων ημερομηνιών έναρξης και λήξης του καθορισμένου [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| τέλος | java.util.Date | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |
| timephasedType | byte | Ο τύπος των δεδομένων χρονικής φάσης ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Λαμβάνει το ποσό του χρονομετρικού έργου για το καθορισμένο χρονικό διάστημα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Αρχή του χρονικού διαστήματος. |
| τέλος | java.util.Date | Τέλος του χρονικού διαστήματος. |

**Returns:**
double - ποσό του χρονοπροσαρμοσμένου έργου για το καθορισμένο χρονικό διάστημα.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Λαμβάνει το ποσό του χρονομετρικού έργου για το καθορισμένο χρονικό διάστημα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Αρχή του χρονικού διαστήματος. |
| τέλος | java.util.Date | Τέλος του χρονικού διαστήματος. |
| timephasedDataType | byte | Τύπος των χρονοπροσαρμοσμένων δεδομένων προς χρήση. |

**Returns:**
double - ποσό του χρονοπροσαρμοσμένου έργου για το καθορισμένο χρονικό διάστημα.
### getUid() {#getUid--}
```
public final int getUid()
```


Λαμβάνει μια τιμή του Uid.

**Returns:**
int - μια τιμή του Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Λαμβάνει μια τιμή του Units.

**Returns:**
double - μια τιμή του Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το UpdateNeeded είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το UpdateNeeded είναι ορισμένο ή όχι.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Λαμβάνει μια τιμή του VAC.

**Returns:**
double - μια τιμή του VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Λαμβάνει μια τιμή του Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Λαμβάνει μια τιμή του WorkContour.

**Returns:**
int - μια τιμή του WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Λαμβάνει μια τιμή του WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Λαμβάνει μια τιμή που υποδεικνύει ότι αυτή η ανάθεση πόρων έχει παιδιά.

**Returns:**
boolean - Πάντα ψευδές.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το παράδειγμα της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Δημιουργεί μια λίστα δεδομένων χρονικής φάσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η καθορισμένη ημερομηνία έναρξης. |
| time | double | Ο καθορισμένος χρόνος εργασίας. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Το καθορισμένο ημερολόγιο εργασίας. |
| λίστα | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | Η λίστα των δεδομένων χρονικής φάσης. |
| isWorking | boolean | Η καθορισμένη σημαία που υποδεικνύει αν τα δεδομένα χρονικής φάσης είναι ενεργά ή όχι. |
| type | int | Ο καθορισμένος τύπος δεδομένων χρονικής φάσης. |

**Returns:**
java.util.Date - Μέγιστη ημερομηνία από τη λίστα ή ημερομηνία έναρξης εάν η λίστα είναι κενή.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Ορίζει μια τιμή του ACWP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Ορίζει μια τιμή του ActualCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Ορίζει μια τιμή του ActualFinish.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του ActualFinish. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Ορίζει μια τιμή του ActualStart.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του ActualStart. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το Confirmed είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το Confirmed είναι ορισμένο ή όχι. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Ορίζει μια τιμή για το Cost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Ορίζει μια τιμή του CostRateTableType.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του CostRateTableType. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Ορίζει μια τιμή του Delay.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Ορίζει ένα παράδειγμα της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο.

--------------------

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | μια παρουσία της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ορίζει μια τιμή για το Finish.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Ορίζει μια τιμή του FinishVariance.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το FixedMaterial είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το FixedMaterial είναι ορισμένο ή όχι. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το HasFixedRateUnits είναι ορισμένο ή όχι. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Ορίζει μοναδικό αναγνωριστικό για αυτήν την ανάθεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.UUID | μοναδικό αναγνωριστικό για αυτήν την ανάθεση. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Ορίζει μια τιμή του Hyperlink.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Ορίζει μια τιμή του HyperlinkAddress.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Ορίζει μια τιμή του HyperlinkSubAddress.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | μια τιμή του HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Ορίζει μια τιμή του LevelingDelay.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το LinkedFields είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το LinkedFields είναι ορισμένο ή όχι. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Ορίζει μονάδες για την ανάθεση ενός υλικού πόρου με μεταβλητή κατανάλωση υλικού. Η μεταβλητή κατανάλωση υλικού σημαίνει ότι καθώς η διάρκεια της ανάθεσης αλλάζει, η ποσότητα των χρησιμοποιούμενων υλικών αλλάζει αναλογικά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μονάδες | double | Αριθμός μονάδων που συσσωρεύονται στην χρονική περίοδο. |
|  | rateScaleType | int | Χρονική περίοδος κατά την οποία συσσωρεύεται η τιμή της μονάδας. |

--------------------

Για παράδειγμα, για να ορίσετε '123/month', πρέπει να κληθεί το SetUnitsScaled(123D, RateScaleType.Month). |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το Milestone είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το Milestone είναι ορισμένο ή όχι. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Ορίζει τις σημειώσεις κειμένου σε μορφή RTF.

--------------------

Υποστηρίζεται μόνο για μορφές MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το κείμενο σημειώσεων σε μορφή RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Ορίζει το απλό κείμενο των σημειώσεων που εξάγεται από τα δεδομένα RTF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | απλό κείμενο των σημειώσεων που εξάγεται από δεδομένα RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Overallocated είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το Overallocated είναι ορισμένο ή όχι. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Ορίζει μια τιμή του OvertimeCost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | μια τιμή του OvertimeCost. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Ορίζει μια τιμή του RateScale.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του RateScale. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


Ο πόρος που έχει ανατεθεί σε μια εργασία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | ο πόρος που έχει εκχωρηθεί σε μια εργασία. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν το ResponsePending είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το ResponsePending είναι ορισμένο ή όχι. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Ορίζει μια τιμή του Resume.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Ορίζει μια τιμή του SV.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ορίζει μια τιμή του Start.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Ορίζει μια τιμή του StartVariance.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Ορίζει μια τιμή του Stop.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή του Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Summary είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το Summary είναι ορισμένο ή όχι. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


Η εργασία στην οποία έχει ανατεθεί ένας πόρος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | η εργασία στην οποία έχει εκχωρηθεί ένας πόρος. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ορίζει το στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στοιχεία του `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) κλάση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | η παρουσία της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) που περιέχει στοιχεία του `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) κλάση. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ορίζει μια τιμή του Uid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Ορίζει μια τιμή του Units.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το UpdateNeeded είναι ορισμένο ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν το UpdateNeeded είναι ορισμένο ή όχι. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Ορίζει μια τιμή του VAC.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | μια τιμή του VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ορίζει μια τιμή του Work.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Ορίζει μια τιμή του WorkContour.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή του WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Ορίζει μια τιμή του WorkVariance.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | μια τιμή του WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Διαιρεί την εργασία σε δύο μέρη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Η αρχή της διακοπής εργασίας για διαχωρισμό βάσει. |
| λήξη | java.util.Date | Το τέλος της διακοπής εργασίας για διαχωρισμό βάσει. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Το ημερολόγιο για διαχωρισμό βάσει. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Δημιουργεί λίστα δεδομένων χρονικής φάσης βάσει της διάρκειας της εργασίας και της προγραμματισμένης ημερομηνίας έναρξης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Το ημερολόγιο για τη δημιουργία δεδομένων χρονοφάσεων από. |

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης [ResourceAssignment](../../com.aspose.tasks/resourceassignment). Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

**Returns:**
java.lang.String - σύντομη συμβολοσειρά που αντιπροσωπεύει το αντικείμενο ανάθεσης.
