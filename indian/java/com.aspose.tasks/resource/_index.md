---
title: "संसाधन"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट में एक संसाधन का प्रतिनिधित्व करता है।"
type: docs
weight: 248
url: /hi/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

प्रोजेक्ट में एक संसाधन का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है। |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है। |
| [canLevel()](#canLevel--) | यह दर्शाने वाला मान प्राप्त करता है कि CanLevel सेट है या नहीं। |
| [delete()](#delete--) | परियोजना से एक संसाधन और उसकी असाइनमेंट्स को हटाता है। |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [Resource](../../com.aspose.tasks/resource) क्लास के इंस्टेंस के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getACWP()](#getACWP--) | ACWP का मान प्राप्त करता है। |
| [getAccrueAt()](#getAccrueAt--) | AccrueAt का मान प्राप्त करता है। |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | ActiveDirectoryGuid का मान प्राप्त करता है। |
| [getActualCost()](#getActualCost--) | ActualCost का मान प्राप्त करता है। |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost का मान प्राप्त करता है। |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork का मान प्राप्त करता है। |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected का मान प्राप्त करता है। |
| [getActualWork()](#getActualWork--) | ActualWork का मान प्राप्त करता है। |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected का मान प्राप्त करता है। |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner का मान प्राप्त करता है। |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid का मान प्राप्त करता है। |
| [getAssignments()](#getAssignments--) | इस ऑब्जेक्ट के लिए संसाधन असाइनमेंट्स का संग्रह प्राप्त करता है। |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) क्लास का इंस्टेंस प्राप्त करता है। |
| [getAvailableFrom()](#getAvailableFrom--) | AvailableFrom का मान प्राप्त करता है। |
| [getAvailableTo()](#getAvailableTo--) | AvailableTo का मान प्राप्त करता है। |
| [getBCWP()](#getBCWP--) | BCWP का मान प्राप्त करता है। |
| [getBCWS()](#getBCWS--) | BCWS का मान प्राप्त करता है। |
| [getBaselines()](#getBaselines--) | इस ऑब्जेक्ट के लिए BaselineCollection का इंस्टेंस प्राप्त करता है। |
| [getBookingType()](#getBookingType--) | BookingType का मान प्राप्त करता है। |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost का मान प्राप्त करता है। |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork का मान प्राप्त करता है। |
| [getCV()](#getCV--) | CV का मान प्राप्त करता है। |
| [getCalendar()](#getCalendar--) | Calendar का मान प्राप्त करता है। |
| [getCode()](#getCode--) | कोड का मान प्राप्त करता है। |
| [getCost()](#getCost--) | लागत का मान प्राप्त करता है। |
| [getCostCenter()](#getCostCenter--) | कॉस्ट सेंटर का मान प्राप्त करता है। |
| [getCostPerUse()](#getCostPerUse--) | प्रति उपयोग लागत का मान प्राप्त करता है। |
| [getCostVariance()](#getCostVariance--) | लागत विचलन का मान प्राप्त करता है। |
| [getCreated()](#getCreated--) | निर्मित का मान प्राप्त करता है। |
| [getEMailAddress()](#getEMailAddress--) | ईमेल पता का मान प्राप्त करता है। |
| [getExtendedAttributes()](#getExtendedAttributes--) | एक विस्तारित विशेषता के मान प्राप्त करता है। |
| [getFinish()](#getFinish--) | समाप्ति का मान प्राप्त करता है। |
| [getGroup()](#getGroup--) | समूह का मान प्राप्त करता है। |
| [getGuid()](#getGuid--) | GUID का मान प्राप्त करता है। |
| [getHyperlink()](#getHyperlink--) | संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ प्राप्त करता है। |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | संसाधन से जुड़े हाइपरलिंक का पता प्राप्त करता है। |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | संसाधन से जुड़े हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को प्राप्त करता है। |
| [getId()](#getId--) | आईडी का मान प्राप्त करता है। |
| [getInactive()](#getInactive--) | यह दर्शाने वाला मान प्राप्त करता है कि निष्क्रिय सेट है या नहीं। |
| [getInitials()](#getInitials--) | प्रारंभिक अक्षरों का मान प्राप्त करता है। |
| [getItems()](#getItems--) | संतान संसाधनों को प्राप्त करता है। |
| [getMaterialLabel()](#getMaterialLabel--) | मैटेरियल लेबल का मान प्राप्त करता है। |
| [getMaxUnits()](#getMaxUnits--) | अधिकतम इकाइयों का मान प्राप्त करता है। |
| [getName()](#getName--) | नाम का मान प्राप्त करता है। |
| [getNotesRTF()](#getNotesRTF--) | नोट्सआरटीएफ का मान प्राप्त करता है। |
| [getNotesText()](#getNotesText--) | नोट्सटेक्स्ट का मान प्राप्त करता है। |
| [getOutlineCode()](#getOutlineCode--) | एक OutlineCodeCollection ऑब्जेक्ट प्राप्त करता है। |
| [getOverallocated()](#getOverallocated--) | यह दर्शाने वाला मान प्राप्त करता है कि ओवरएलोकेटेड सेट है या नहीं। |
| [getOvertimeCost()](#getOvertimeCost--) | ओवरटाइमकॉस्ट का मान प्राप्त करता है। |
| [getOvertimeRate()](#getOvertimeRate--) | ओवरटाइमरेट का मान प्राप्त करता है। |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | ओवरटाइमरेटफ़ॉर्मेट का मान प्राप्त करता है। |
| [getOvertimeWork()](#getOvertimeWork--) | ओवरटाइमवर्क का मान प्राप्त करता है। |
| [getParentProject()](#getParentProject--) | इस कंटेनर के लिए पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [getPeakUnits()](#getPeakUnits--) | पीकयूनिट्स का मान प्राप्त करता है। |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | परसेंटवर्ककम्प्लीट का मान प्राप्त करता है। |
| [getPhonetics()](#getPhonetics--) | फ़ोनेटिक्स का मान प्राप्त करता है। |
| [getRates()](#getRates--) | इस ऑब्जेक्ट के लिए [RateCollection](../../com.aspose.tasks/ratecollection) क्लास का एक इंस्टेंस प्राप्त करता है। |
| [getRegularWork()](#getRegularWork--) | रेगुलरवर्क का मान प्राप्त करता है। |
| [getRemainingCost()](#getRemainingCost--) | रिमेनिंगकॉस्ट का मान प्राप्त करता है। |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | रिमेनिंगओवरटाइमकॉस्ट का मान प्राप्त करता है। |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | रिमेनिंगओवरटाइमवर्क का मान प्राप्त करता है। |
| [getRemainingWork()](#getRemainingWork--) | रिमेनिंगवर्क का मान प्राप्त करता है। |
| [getSV()](#getSV--) | एसवी का मान प्राप्त करता है। |
| [getStandardRate()](#getStandardRate--) | स्टैंडर्डरेट का मान प्राप्त करता है। |
| [getStandardRateFormat()](#getStandardRateFormat--) | स्टैंडर्डरेटफ़ॉर्मेट का मान प्राप्त करता है। |
| [getStart()](#getStart--) | स्टार्ट का मान प्राप्त करता है। |
| [getTimephasedData()](#getTimephasedData--) | इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का एक इंस्टेंस प्राप्त करता है। |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) लौटाता है जिसमें `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) मान दिए गए प्रारंभ और समाप्ति तिथियों के भीतर होते हैं। |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का एक इंस्टेंस लौटाता है जिसमें `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) मान निर्दिष्ट [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) की दी गई प्रारंभ और समाप्ति तिथियों के भीतर होते हैं। |
| [getType()](#getType--) | टाइप का मान प्राप्त करता है। |
| [getUid()](#getUid--) | यूआईडी का मान प्राप्त करता है। |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | विंडोज़यूज़रएकाउंट का मान प्राप्त करता है। |
| [getWork()](#getWork--) | वर्क का मान प्राप्त करता है। |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance का मान प्राप्त करता है। |
| [getWorkgroup()](#getWorkgroup--) | Workgroup का मान प्राप्त करता है। |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | इंस्टेंस के लिए हैश कोड मान लौटाता है [Resource](../../com.aspose.tasks/resource) क्लास का। |
| [isBudget()](#isBudget--) | IsBudget सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isCostResource()](#isCostResource--) | IsCostResource सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isEnterprise()](#isEnterprise--) | IsEnterprise सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isGeneric()](#isGeneric--) | IsGeneric सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isNull()](#isNull--) | IsNull सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isRoot()](#isRoot--) | resource मूल संसाधन है या नहीं, यह दर्शाने वाला फ़्लैग प्राप्त करता है। |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | IsTeamAssignmentPool सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है। |
| [setACWP(double value)](#setACWP-double-) | ACWP का मान सेट करता है। |
| [setAccrueAt(int value)](#setAccrueAt-int-) | AccrueAt का मान सेट करता है। |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | ActiveDirectoryGuid का मान सेट करता है। |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost का मान सेट करता है। |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost का मान सेट करता है। |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork का मान सेट करता है। |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected का मान सेट करता है। |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork का मान सेट करता है। |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected का मान सेट करता है। |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner का मान सेट करता है। |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid का मान सेट करता है। |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | AvailableFrom का मान सेट करता है। |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | AvailableTo का मान सेट करता है। |
| [setBCWP(double value)](#setBCWP-double-) | BCWP का मान सेट करता है। |
| [setBCWS(double value)](#setBCWS-double-) | BCWS का मान सेट करता है। |
| [setBookingType(int value)](#setBookingType-int-) | BookingType का मान सेट करता है। |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | IsBudget सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost का मान सेट करता है। |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork का मान सेट करता है। |
| [setCV(double value)](#setCV-double-) | CV का मान सेट करता है। |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar का मान सेट करता है। |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | CanLevel सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setCode(String value)](#setCode-java.lang.String-) | Code का मान सेट करता है। |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost का मान सेट करता है। |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | CostCenter का मान सेट करता है। |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | CostPerUse का मान सेट करता है। |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | IsCostResource सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance का मान सेट करता है। |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created का मान सेट करता है। |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | EMailAddress का मान सेट करता है। |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | IsEnterprise सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish का मान सेट करता है। |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | IsGeneric सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setGroup(String value)](#setGroup-java.lang.String-) | Group का मान सेट करता है। |
| [setGuid(String value)](#setGuid-java.lang.String-) | Guid का मान सेट करता है। |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ सेट करता है। |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | संसाधन से जुड़े हाइपरलिंक का पता सेट करता है। |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | संसाधन से जुड़े हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को सेट करता है। |
| [setId(int value)](#setId-int-) | Id का मान सेट करता है। |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Inactive सेट है या नहीं, यह दर्शाते हुए मान सेट करता है। |
| [setInitials(String value)](#setInitials-java.lang.String-) | Initials का मान सेट करता है। |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | MaterialLabel का मान सेट करता है। |
| [setMaxUnits(double value)](#setMaxUnits-double-) | MaxUnits का मान सेट करता है। |
| [setName(String value)](#setName-java.lang.String-) | Name का मान सेट करता है। |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | NotesRTF का मान सेट करता है। |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | NotesText का मान सेट करता है। |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | IsNull सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Overallocated सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost का मान सेट करता है। |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | OvertimeRate का मान सेट करता है। |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | OvertimeRateFormat का मान सेट करता है। |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork का मान सेट करता है। |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits का मान सेट करता है। |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete का मान सेट करता है। |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Phonetics का मान सेट करता है। |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork का मान सेट करता है। |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost का मान सेट करता है। |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost का मान सेट करता है। |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork का मान सेट करता है। |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork का मान सेट करता है। |
| [setSV(double value)](#setSV-double-) | SV का मान सेट करता है। |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | StandardRate का मान सेट करता है। |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | StandardRateFormat का मान सेट करता है। |
| [setStart(Date value)](#setStart-java.util.Date-) | Start का मान सेट करता है। |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | IsTeamAssignmentPool सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास की एक इंस्टेंस सेट करता है। |
| [setType(int value)](#setType-int-) | Type का मान सेट करता है। |
| [setUid(int value)](#setUid-int-) | Uid का मान सेट करता है। |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | WindowsUserAccount का मान सेट करता है। |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work का मान सेट करता है। |
| [setWorkVariance(double value)](#setWorkVariance-double-) | WorkVariance का मान सेट करता है। |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Workgroup का मान सेट करता है। |
| [toString()](#toString--) | [Resource](../../com.aspose.tasks/resource) क्लास की इंस्टेंस का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Rsc](../../com.aspose.tasks/rsc)। |

**Returns:**
T - वह मान जिससे इस कंटेनर में प्रॉपर्टी मैप की गई है।
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Rsc](../../com.aspose.tasks/rsc)। |
| मान | T | मान। |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


यह दर्शाने वाला मान प्राप्त करता है कि CanLevel सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


परियोजना से एक संसाधन और उसकी असाइनमेंट्स को हटाता है।

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [Resource](../../com.aspose.tasks/resource) क्लास के इंस्टेंस के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | इस इंस्टेंस की तुलना करने के लिए निर्दिष्ट [Resource](../../com.aspose.tasks/resource) क्लास की इंस्टेंस। |

**Returns:**
boolean - यदि निर्दिष्ट [Resource](../../com.aspose.tasks/resource) क्लास की इंस्टेंस का Uid मान इस इंस्टेंस के समान है तो **True**, अन्यथा **false**।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
boolean - यदि निर्दिष्ट ऑब्जेक्ट एक Resource है जिसका Uid मान इस इंस्टेंस के समान है तो **True**, अन्यथा **false**।
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP का मान प्राप्त करता है।

**Returns:**
double - ACWP का मान।
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


AccrueAt का मान प्राप्त करता है।

**Returns:**
int - AccrueAt का मान।
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


ActiveDirectoryGuid का मान प्राप्त करता है।

**Returns:**
java.lang.String - ActiveDirectoryGuid का मान।
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - ActualCost का मान।
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - ActualOvertimeCost का मान।
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner का मान प्राप्त करता है।

**Returns:**
java.lang.String - AssignmentOwner का मान।
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid का मान प्राप्त करता है।

**Returns:**
java.lang.String - AssignmentOwnerGuid का मान।
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


इस ऑब्जेक्ट के लिए संसाधन असाइनमेंट्स का संग्रह प्राप्त करता है।

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) क्लास की इंस्टेंस प्राप्त करता है। वह अवधि संग्रह जिसमें एक रिसोर्स उपलब्ध रहता है।

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


AvailableFrom का मान प्राप्त करता है।

**Returns:**
java.util.Date - AvailableFrom का मान।
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


AvailableTo का मान प्राप्त करता है।

**Returns:**
java.util.Date - AvailableTo का मान।
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP का मान प्राप्त करता है।

**Returns:**
double - BCWP का मान।
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS का मान प्राप्त करता है।

**Returns:**
double - BCWS का मान।
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


इस ऑब्जेक्ट के लिए BaselineCollection का एक इंस्टेंस प्राप्त करता है। एक संसाधन के लिए बेसलाइन मान।

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType का मान प्राप्त करता है।

**Returns:**
int - BookingType का मान।
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - BudgetCost का मान।
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV का मान प्राप्त करता है।

**Returns:**
double - CV का मान।
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar का मान प्राप्त करता है।

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


कोड का मान प्राप्त करता है।

**Returns:**
java.lang.String - Code का मान।
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - Cost का मान।
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


कॉस्ट सेंटर का मान प्राप्त करता है।

**Returns:**
java.lang.String - CostCenter का मान।
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


प्रति उपयोग लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - CostPerUse का मान।
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


लागत विचलन का मान प्राप्त करता है।

**Returns:**
double - CostVariance का मान।
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


निर्मित का मान प्राप्त करता है।

**Returns:**
java.util.Date - Created का मान।
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


ईमेल पता का मान प्राप्त करता है।

**Returns:**
java.lang.String - EMailAddress का मान।
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


एक विस्तारित विशेषता के मान प्राप्त करता है।

--------------------

दो डेटा टुकड़े आवश्यक हैं - एक पॉइंटर जो विस्तारित एट्रिब्यूट टेबल की ओर वापस जाता है जिसे या तो यूनिक ID या फ़ील्ड ID द्वारा निर्दिष्ट किया गया है, और वह मान जो या तो मान के साथ निर्दिष्ट किया गया है, या मान सूची की ओर वापस जाने वाला पॉइंटर।

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


समाप्ति का मान प्राप्त करता है।

**Returns:**
java.util.Date - Finish का मान।
### getGroup() {#getGroup--}
```
public final String getGroup()
```


समूह का मान प्राप्त करता है।

**Returns:**
java.lang.String - Group का मान।
### getGuid() {#getGuid--}
```
public final String getGuid()
```


GUID का मान प्राप्त करता है।

**Returns:**
java.lang.String - Guid का मान।
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ प्राप्त करता है।

**Returns:**
java.lang.String - संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ।
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


संसाधन से जुड़े हाइपरलिंक का पता प्राप्त करता है।

--------------------

हाइपरलिंक का पूरा पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress के संयोजन से बनता है।

**Returns:**
java.lang.String - संसाधन से जुड़े हाइपरलिंक का पता।
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


संसाधन से जुड़े हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को प्राप्त करता है।

--------------------

हाइपरलिंक का पूरा पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress के संयोजन से बनता है।

**Returns:**
java.lang.String - संसाधन से जुड़े हाइपरलिंक में दस्तावेज़ के भीतर विशिष्ट स्थान।
### getId() {#getId--}
```
public final int getId()
```


आईडी का मान प्राप्त करता है।

**Returns:**
int - Id का मान।
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


यह दर्शाने वाला मान प्राप्त करता है कि निष्क्रिय सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


प्रारंभिक अक्षरों का मान प्राप्त करता है।

**Returns:**
java.lang.String - Initials का मान।
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


संतान संसाधनों को प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - संतान संसाधन।
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


मैटेरियल लेबल का मान प्राप्त करता है।

**Returns:**
java.lang.String - MaterialLabel का मान।
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


अधिकतम इकाइयों का मान प्राप्त करता है।

**Returns:**
double - MaxUnits का मान।
### getName() {#getName--}
```
public final String getName()
```


नाम का मान प्राप्त करता है।

**Returns:**
java.lang.String - Name का मान।
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


नोट्सआरटीएफ का मान प्राप्त करता है।

**Returns:**
java.lang.String - NotesRTF का मान।
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


नोट्सटेक्स्ट का मान प्राप्त करता है।

**Returns:**
java.lang.String - NotesText का मान।
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


OutlineCodeCollection ऑब्जेक्ट प्राप्त करता है। आउटलाइन कोड का मान।

--------------------

दो डेटा टुकड़े आवश्यक हैं - FieldID द्वारा निर्दिष्ट आउटलाइन कोड तालिका के लिए एक पॉइंटर, और वह मान जो ValueID या ValueGUID पॉइंटर द्वारा मान सूची में निर्दिष्ट किया गया है।

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


यह दर्शाने वाला मान प्राप्त करता है कि ओवरएलोकेटेड सेट है या नहीं।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


ओवरटाइमकॉस्ट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - OvertimeCost का मान।
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


ओवरटाइमरेट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - OvertimeRate का मान।
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


ओवरटाइमरेटफ़ॉर्मेट का मान प्राप्त करता है।

**Returns:**
int - OvertimeRateFormat का मान।
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


ओवरटाइमवर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


इस कंटेनर के लिए पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


पीकयूनिट्स का मान प्राप्त करता है।

**Returns:**
double - PeakUnits का मान।
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


परसेंटवर्ककम्प्लीट का मान प्राप्त करता है।

**Returns:**
int - PercentWorkComplete का मान।
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


फ़ोनेटिक्स का मान प्राप्त करता है।

**Returns:**
java.lang.String - Phonetics का मान।
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


[RateCollection](../../com.aspose.tasks/ratecollection) क्लास की इस ऑब्जेक्ट के लिए एक इंस्टेंस प्राप्त करता है। प्रत्येक के साथ जुड़े अवधियों और दरों का संग्रह।

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


रेगुलरवर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


रिमेनिंगकॉस्ट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - RemainingCost का मान।
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


रिमेनिंगओवरटाइमकॉस्ट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost का मान।
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


रिमेनिंगओवरटाइमवर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


रिमेनिंगवर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


एसवी का मान प्राप्त करता है।

**Returns:**
double - SV का मान।
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


स्टैंडर्डरेट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - StandardRate का मान।
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


स्टैंडर्डरेटफ़ॉर्मेट का मान प्राप्त करता है।

**Returns:**
int - StandardRateFormat का मान।
### getStart() {#getStart--}
```
public final Date getStart()
```


स्टार्ट का मान प्राप्त करता है।

**Returns:**
java.util.Date - Start का मान।
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का एक इंस्टेंस प्राप्त करता है।

--------------------

केवल XML प्रारूप के लिए पढ़ना समर्थित है।

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) लौटाता है जिसमें `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) मान दिए गए प्रारंभ और समाप्ति तिथियों के भीतर होते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | समय-फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| समाप्ति | java.util.Date | समय‑फ़ेज़्ड डेटा की समाप्ति तिथि। |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का एक इंस्टेंस लौटाता है जिसमें `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) मान निर्दिष्ट [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) की दी गई प्रारंभ और समाप्ति तिथियों के भीतर होते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | समय‑फ़ेज़्ड डेटा की प्रारंभ तिथि। |
| समाप्ति | java.util.Date | समय‑फ़ेज़्ड डेटा की समाप्ति तिथि। |
| timephasedType | byte | समय‑फ़ेज़्ड डेटा का प्रकार ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


टाइप का मान प्राप्त करता है।

**Returns:**
int - Type का मान।
### getUid() {#getUid--}
```
public final int getUid()
```


यूआईडी का मान प्राप्त करता है।

**Returns:**
int - Uid का मान।
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


विंडोज़यूज़रएकाउंट का मान प्राप्त करता है।

**Returns:**
java.lang.String - WindowsUserAccount का मान।
### getWork() {#getWork--}
```
public final Duration getWork()
```


वर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


WorkVariance का मान प्राप्त करता है।

**Returns:**
double - WorkVariance का मान।
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Workgroup का मान प्राप्त करता है।

**Returns:**
int - Workgroup का मान।
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


आंतरिक उपयोग के लिए आरक्षित।

**Returns:**
बूलियन - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


इंस्टेंस के लिए हैश कोड मान लौटाता है [Resource](../../com.aspose.tasks/resource) क्लास का।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


IsBudget सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


IsCostResource सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


IsEnterprise सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


IsGeneric सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


IsNull सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


संसाधन एक मूल संसाधन है या नहीं, यह दर्शाने वाला फ़्लैग प्राप्त करता है। मूल संसाधन एक विशेष संसाधन है जो MS Project के फ़ॉर्मेट के आंतरिक भागों को समर्थन देने के लिए अभिप्रेत है और उपयोगकर्ता के कोड से सीधे उपयोग करने के लिए नहीं है।

**Returns:**
boolean - वह फ़्लैग जो दर्शाता है कि संसाधन मूल संसाधन है या नहीं।
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


IsTeamAssignmentPool सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - वह मान जो दर्शाता है कि IsTeamAssignmentPool सेट है या नहीं।
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Rsc](../../com.aspose.tasks/rsc)। |
| मान | java.util.Date | मान। |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | ACWP का मान। |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


AccrueAt का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | AccrueAt का मान। |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


ActiveDirectoryGuid का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | ActiveDirectoryGuid का मान। |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | ActualCost का मान। |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | ActualOvertimeCost का मान। |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork का मान। |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected का मान। |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork का मान। |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected का मान। |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | AssignmentOwner का मान। |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | AssignmentOwnerGuid का मान। |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


AvailableFrom का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | AvailableFrom का मान। |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


AvailableTo का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | AvailableTo का मान। |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | BCWP का मान। |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | BCWS का मान। |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | BookingType का मान। |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


IsBudget सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsBudget सेट है या नहीं, यह दर्शाने वाला मान। |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | BudgetCost का मान। |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork का मान। |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | CV का मान। |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Calendar का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | Calendar का मान। |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


CanLevel सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | CanLevel सेट है या नहीं, यह दर्शाने वाला मान। |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Code का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Code का मान। |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | Cost का मान। |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


CostCenter का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | CostCenter का मान। |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


CostPerUse का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | CostPerUse का मान। |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


IsCostResource सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsCostResource सेट है या नहीं, यह दर्शाने वाला मान। |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | CostVariance का मान। |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Created का मान। |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


EMailAddress का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | EMailAddress का मान। |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


IsEnterprise सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsEnterprise सेट है या नहीं, यह दर्शाने वाला मान। |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Finish का मान। |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


IsGeneric सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsGeneric सेट है या नहीं, यह दर्शाने वाला मान। |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Group का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Group का मान। |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Guid का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Guid का मान। |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | संसाधन से जुड़ी हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ। |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


संसाधन से जुड़े हाइपरलिंक का पता सेट करता है।

--------------------

हाइपरलिंक का पूरा पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress के संयोजन से बनता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | संसाधन से जुड़ी एक हाइपरलिंक के लिए पता। |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


संसाधन से जुड़े हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को सेट करता है।

--------------------

हाइपरलिंक का पूरा पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress के संयोजन से बनता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | संसाधन से जुड़ी एक हाइपरलिंक में दस्तावेज़ के भीतर विशिष्ट स्थान। |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Id का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Id का मान। |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Inactive सेट है या नहीं, यह दर्शाते हुए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | यह दर्शाने वाला मान कि Inactive सेट है या नहीं। |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Initials का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Initials का मान। |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


MaterialLabel का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | MaterialLabel का मान। |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


MaxUnits का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | MaxUnits का मान। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Name का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Name का मान। |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


NotesRTF का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | NotesRTF का मान। |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


NotesText का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | NotesText का मान। |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


IsNull सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | यह दर्शाने वाला मान कि IsNull सेट है या नहीं। |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Overallocated सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | यह दर्शाने वाला मान कि Overallocated सेट है या नहीं। |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | OvertimeCost का मान। |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


OvertimeRate का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | OvertimeRate का मान। |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


OvertimeRateFormat का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | OvertimeRateFormat का मान। |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork का मान। |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | PeakUnits का मान। |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | PercentWorkComplete का मान। |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Phonetics का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Phonetics का मान। |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork का मान। |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | RemainingCost का मान। |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | RemainingOvertimeCost का मान। |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork का मान। |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork का मान। |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | SV का मान। |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


StandardRate का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | StandardRate का मान। |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


StandardRateFormat का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | StandardRateFormat का मान। |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Start का मान। |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


IsTeamAssignmentPool सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | IsTeamAssignmentPool सेट है या नहीं, यह दर्शाने वाला मान। |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास की एक इंस्टेंस सेट करता है।

--------------------

केवल XML प्रारूप के लिए पढ़ना समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | इस ऑब्जेक्ट के लिए [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का एक उदाहरण। |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Type का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Type का मान। |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Uid का मान। |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


WindowsUserAccount का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | WindowsUserAccount का मान। |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work का मान। |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


WorkVariance का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | WorkVariance का मान। |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Workgroup का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Workgroup का मान। |

### toString() {#toString--}
```
public String toString()
```


यह [Resource](../../com.aspose.tasks/resource) क्लास के इंस्टेंस का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं।

**Returns:**
java.lang.String - वह संक्षिप्त स्ट्रिंग जो रिसोर्स ऑब्जेक्ट का प्रतिनिधित्व करती है।
