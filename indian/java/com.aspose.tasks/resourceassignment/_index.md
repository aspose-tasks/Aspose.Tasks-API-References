---
title: "ResourceAssignment"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट में एक संसाधन असाइनमेंट का प्रतिनिधित्व करता है।"
type: docs
weight: 249
url: /hi/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

प्रोजेक्ट में एक संसाधन असाइनमेंट का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है। |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है। |
| [delete()](#delete--) | परियोजना असाइनमेंट संग्रह से संसाधन असाइनमेंट को हटाता है। |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट [ResourceAssignment](../../com.aspose.tasks/resourceassignment) वर्ग के उदाहरण के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getACWP()](#getACWP--) | ACWP का मान प्राप्त करता है। |
| [getActualCost()](#getActualCost--) | ActualCost का मान प्राप्त करता है। |
| [getActualFinish()](#getActualFinish--) | ActualFinish का मान प्राप्त करता है। |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost का मान प्राप्त करता है। |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork का मान प्राप्त करता है। |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected का मान प्राप्त करता है। |
| [getActualStart()](#getActualStart--) | ActualStart का मान प्राप्त करता है। |
| [getActualWork()](#getActualWork--) | ActualWork का मान प्राप्त करता है। |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected का मान प्राप्त करता है। |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner का मान प्राप्त करता है। |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid का मान प्राप्त करता है। |
| [getBCWP()](#getBCWP--) | BCWP का मान प्राप्त करता है। |
| [getBCWS()](#getBCWS--) | BCWS का मान प्राप्त करता है। |
| [getBaselines()](#getBaselines--) | AssignmentBaselineCollection ऑब्जेक्ट प्राप्त करता है। |
| [getBookingType()](#getBookingType--) | BookingType का मान प्राप्त करता है। |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost का मान प्राप्त करता है। |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork का मान प्राप्त करता है। |
| [getCV()](#getCV--) | CV का मान प्राप्त करता है। |
| [getConfirmed()](#getConfirmed--) | एक मान प्राप्त करता है जो दर्शाता है कि Confirmed सेट है या नहीं। |
| [getCost()](#getCost--) | लागत का मान प्राप्त करता है। |
| [getCostRateTableType()](#getCostRateTableType--) | CostRateTableType का मान प्राप्त करता है। |
| [getCostVariance()](#getCostVariance--) | लागत विचलन का मान प्राप्त करता है। |
| [getCreated()](#getCreated--) | निर्मित का मान प्राप्त करता है। |
| [getDelay()](#getDelay--) | Delay का मान प्राप्त करता है। |
| [getExtendedAttributes()](#getExtendedAttributes--) | इस ऑब्जेक्ट के लिए ExtendedAttributeCollection वर्ग का एक उदाहरण प्राप्त करता है। |
| [getFinish()](#getFinish--) | समाप्ति का मान प्राप्त करता है। |
| [getFinishVariance()](#getFinishVariance--) | FinishVariance का मान प्राप्त करता है। |
| [getFixedMaterial()](#getFixedMaterial--) | एक मान प्राप्त करता है जो यह दर्शाता है कि FixedMaterial सेट है या नहीं। |
| [getGuid()](#getGuid--) | इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [getHyperlink()](#getHyperlink--) | Hyperlink का मान प्राप्त करता है। |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | HyperlinkAddress का मान प्राप्त करता है। |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | HyperlinkSubAddress का मान प्राप्त करता है। |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | LevelingDelay का मान प्राप्त करता है। |
| [getLinkedFields()](#getLinkedFields--) | एक मान प्राप्त करता है जो यह दर्शाता है कि LinkedFields सेट है या नहीं। |
| [getMilestone()](#getMilestone--) | एक मान प्राप्त करता है जो यह दर्शाता है कि Milestone सेट है या नहीं। |
| [getNotesRTF()](#getNotesRTF--) | RTF स्वरूप में पाठ नोट्स प्राप्त करता है। |
| [getNotesText()](#getNotesText--) | RTF डेटा से निकाले गए नोट्स का साधारण पाठ प्राप्त करता है। |
| [getOverallocated()](#getOverallocated--) | यह दर्शाने वाला मान प्राप्त करता है कि ओवरएलोकेटेड सेट है या नहीं। |
| [getOvertimeCost()](#getOvertimeCost--) | ओवरटाइमकॉस्ट का मान प्राप्त करता है। |
| [getOvertimeWork()](#getOvertimeWork--) | ओवरटाइमवर्क का मान प्राप्त करता है। |
| [getParentProject()](#getParentProject--) | इस असाइनमेंट के लिए पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [getPeakUnits()](#getPeakUnits--) | पीकयूनिट्स का मान प्राप्त करता है। |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | परसेंटवर्ककम्प्लीट का मान प्राप्त करता है। |
| [getRateScale()](#getRateScale--) | RateScale का मान प्राप्त करता है। |
| [getRegularWork()](#getRegularWork--) | रेगुलरवर्क का मान प्राप्त करता है। |
| [getRemainingCost()](#getRemainingCost--) | रिमेनिंगकॉस्ट का मान प्राप्त करता है। |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | रिमेनिंगओवरटाइमकॉस्ट का मान प्राप्त करता है। |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | रिमेनिंगओवरटाइमवर्क का मान प्राप्त करता है। |
| [getRemainingWork()](#getRemainingWork--) | रिमेनिंगवर्क का मान प्राप्त करता है। |
| [getResource()](#getResource--) | एक कार्य को सौंपा गया संसाधन। |
| [getResponsePending()](#getResponsePending--) | एक मान प्राप्त करता है जो यह दर्शाता है कि ResponsePending सेट है या नहीं। |
| [getResume()](#getResume--) | Resume का मान प्राप्त करता है। |
| [getSV()](#getSV--) | एसवी का मान प्राप्त करता है। |
| [getStart()](#getStart--) | स्टार्ट का मान प्राप्त करता है। |
| [getStartVariance()](#getStartVariance--) | StartVariance का मान प्राप्त करता है। |
| [getStop()](#getStop--) | Stop का मान प्राप्त करता है। |
| [getSummary()](#getSummary--) | एक मान प्राप्त करता है जो यह दर्शाता है कि Summary सेट है या नहीं। |
| [getTask()](#getTask--) | वह कार्य जिससे एक संसाधन सौंपा गया है। |
| [getTimephasedData()](#getTimephasedData--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का वह इंस्टेंस प्राप्त करता है जिसमें `TimephasedData` के तत्व होते हैं ([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) क्लास। |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ऑब्जेक्ट को `TimephasedData` के इंस्टेंस के साथ लौटाता है ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) क्लास, जो दिए गए प्रारंभ और समाप्ति तिथियों के भीतर [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) के होते हैं। |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | निर्दिष्ट [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) के दिए गए प्रारंभ और समाप्ति तिथियों के भीतर `TimephasedData` के इंस्टेंस वाले [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का इंस्टेंस लौटाता है ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) क्लास। |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है। |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है। |
| [getUid()](#getUid--) | यूआईडी का मान प्राप्त करता है। |
| [getUnits()](#getUnits--) | Units का मान प्राप्त करता है। |
| [getUpdateNeeded()](#getUpdateNeeded--) | एक मान प्राप्त करता है जो यह दर्शाता है कि UpdateNeeded सेट है या नहीं। |
| [getVAC()](#getVAC--) | VAC का मान प्राप्त करता है। |
| [getWork()](#getWork--) | वर्क का मान प्राप्त करता है। |
| [getWorkContour()](#getWorkContour--) | WorkContour का मान प्राप्त करता है। |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance का मान प्राप्त करता है। |
| [hasChildren()](#hasChildren--) | इस संसाधन असाइनमेंट में बच्चों के होने का संकेत देने वाला मान प्राप्त करता है। |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | HasFixedRateUnits सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [hashCode()](#hashCode--) | यह [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास के उदाहरण के लिए हैश कोड मान लौटाता है। |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | समय-फ़ेज़ डेटा की सूची उत्पन्न करता है। |
| [setACWP(double value)](#setACWP-double-) | ACWP का मान सेट करता है। |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost का मान सेट करता है। |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | ActualFinish का मान सेट करता है। |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost का मान सेट करता है। |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork का मान सेट करता है। |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected का मान सेट करता है। |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | ActualStart का मान सेट करता है। |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork का मान सेट करता है। |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected का मान सेट करता है। |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner का मान सेट करता है। |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid का मान सेट करता है। |
| [setBCWP(double value)](#setBCWP-double-) | BCWP का मान सेट करता है। |
| [setBCWS(double value)](#setBCWS-double-) | BCWS का मान सेट करता है। |
| [setBookingType(int value)](#setBookingType-int-) | BookingType का मान सेट करता है। |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost का मान सेट करता है। |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork का मान सेट करता है। |
| [setCV(double value)](#setCV-double-) | CV का मान सेट करता है। |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Confirmed सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost का मान सेट करता है। |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | CostRateTableType का मान सेट करता है। |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance का मान सेट करता है। |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created का मान सेट करता है। |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Delay का मान सेट करता है। |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | इस ऑब्जेक्ट के लिए ExtendedAttributeCollection क्लास का एक उदाहरण सेट करता है। |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish का मान सेट करता है। |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | FinishVariance का मान सेट करता है। |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | FixedMaterial सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | HasFixedRateUnits सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता सेट करता है। |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Hyperlink का मान सेट करता है। |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | HyperlinkAddress का मान सेट करता है। |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | HyperlinkSubAddress का मान सेट करता है। |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | LevelingDelay का मान सेट करता है। |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | LinkedFields सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | परिवर्तनीय सामग्री खपत वाले सामग्री संसाधन के असाइनमेंट के लिए इकाइयों को सेट करता है। |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Milestone सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | RTF प्रारूप में टेक्स्ट नोट्स सेट करता है। |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | RTF डेटा से निकाले गए नोट्स का साधारण टेक्स्ट सेट करता है। |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Overallocated सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost का मान सेट करता है। |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork का मान सेट करता है। |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits का मान सेट करता है। |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete का मान सेट करता है। |
| [setRateScale(int value)](#setRateScale-int-) | RateScale का मान सेट करता है। |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork का मान सेट करता है। |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost का मान सेट करता है। |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost का मान सेट करता है। |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork का मान सेट करता है। |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork का मान सेट करता है। |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | एक कार्य को सौंपा गया संसाधन। |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | ResponsePending सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setResume(Date value)](#setResume-java.util.Date-) | Resume का मान सेट करता है। |
| [setSV(double value)](#setSV-double-) | SV का मान सेट करता है। |
| [setStart(Date value)](#setStart-java.util.Date-) | Start का मान सेट करता है। |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | StartVariance का मान सेट करता है। |
| [setStop(Date value)](#setStop-java.util.Date-) | Stop का मान सेट करता है। |
| [setSummary(boolean value)](#setSummary-boolean-) | Summary सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | वह कार्य जिससे एक संसाधन सौंपा गया है। |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास की वह इंस्टेंस सेट करता है जिसमें `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) तत्व होते हैं। |
| [setUid(int value)](#setUid-int-) | Uid का मान सेट करता है। |
| [setUnits(double value)](#setUnits-double-) | Units का मान सेट करता है। |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | UpdateNeeded सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setVAC(double value)](#setVAC-double-) | VAC का मान सेट करता है। |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work का मान सेट करता है। |
| [setWorkContour(int value)](#setWorkContour-int-) | WorkContour का मान सेट करता है। |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | WorkVariance का मान सेट करता है। |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | टास्क को दो भागों में विभाजित करता है। |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | टास्क की अवधि और निर्धारित प्रारंभ तिथि के आधार पर टाइम-फेज़्ड डेटा की सूची उत्पन्न करता है। |
| [toString()](#toString--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास की इंस्टेंस का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Asn](../../com.aspose.tasks/asn) का उपयोग करें। |

**Returns:**
T - वह मान जिससे इस कंटेनर में प्रॉपर्टी मैप की गई है।
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [Asn](../../com.aspose.tasks/asn) का उपयोग करें। |
| मान | T | मान। |

### delete() {#delete--}
```
public final void delete()
```


परियोजना असाइनमेंट संग्रह से संसाधन असाइनमेंट को हटाता है।

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट [ResourceAssignment](../../com.aspose.tasks/resourceassignment) वर्ग के उदाहरण के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास की इंस्टेंस। |

**Returns:**
boolean - यदि निर्दिष्ट [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास की इंस्टेंस का UID मान इस इंस्टेंस के समान है तो **True**, अन्यथा **false**।
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
boolean - यदि o एक ResourceAssignment है जो इस इंस्टेंस के समान रिसोर्स और टास्क असाइन करता है तो **True**, अन्यथा **false**।
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP का मान प्राप्त करता है।

**Returns:**
double - ACWP का मान।
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - ActualCost का मान।
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


ActualFinish का मान प्राप्त करता है।

**Returns:**
java.util.Date - ActualFinish का मान।
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


ActualStart का मान प्राप्त करता है।

**Returns:**
java.util.Date - ActualStart का मान।
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
public final AssignmentBaselineCollection getBaselines()
```


AssignmentBaselineCollection ऑब्जेक्ट प्राप्त करता है। असाइनमेंट से जुड़े बेसलाइन मानों का संग्रह।

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


एक मान प्राप्त करता है जो दर्शाता है कि Confirmed सेट है या नहीं।

**Returns:**
boolean - दर्शाता है कि Confirmed सेट है या नहीं।
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - Cost का मान।
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


CostRateTableType का मान प्राप्त करता है।

**Returns:**
int - CostRateTableType का मान।
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Delay का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


इस ऑब्जेक्ट के लिए ExtendedAttributeCollection वर्ग का एक उदाहरण प्राप्त करता है।

--------------------

केवल XML प्रारूप के लिए पढ़ना समर्थित है।

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


समाप्ति का मान प्राप्त करता है।

**Returns:**
java.util.Date - Finish का मान।
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


FinishVariance का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि FixedMaterial सेट है या नहीं।

**Returns:**
boolean - दर्शाता है कि FixedMaterial सेट है या नहीं।
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता प्राप्त करता है।

**Returns:**
java.util.UUID - इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता।
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hyperlink का मान प्राप्त करता है।

**Returns:**
java.lang.String - Hyperlink का मान।
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


HyperlinkAddress का मान प्राप्त करता है।

**Returns:**
java.lang.String - HyperlinkAddress का मान।
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


HyperlinkSubAddress का मान प्राप्त करता है।

**Returns:**
java.lang.String - HyperlinkSubAddress का मान।
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


आंतरिक उपयोग के लिए आरक्षित।

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


LevelingDelay का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि LinkedFields सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि LinkedFields सेट है या नहीं।
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि Milestone सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि Milestone सेट है या नहीं।
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


RTF स्वरूप में पाठ नोट्स प्राप्त करता है।

--------------------

केवल MPP फ़ॉर्मेट्स के लिए समर्थित।

**Returns:**
java.lang.String - RTF स्वरूप में पाठ नोट्स।
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


RTF डेटा से निकाले गए नोट्स का साधारण पाठ प्राप्त करता है।

**Returns:**
java.lang.String - RTF डेटा से निकाला गया नोट्स का साधारण पाठ।
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


यह दर्शाने वाला मान प्राप्त करता है कि ओवरएलोकेटेड सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि Overallocated सेट है या नहीं।
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


ओवरटाइमकॉस्ट का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - OvertimeCost का मान।
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


इस असाइनमेंट के लिए पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


RateScale का मान प्राप्त करता है।

**Returns:**
int - RateScale का मान।
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


एक कार्य को सौंपा गया संसाधन।

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि ResponsePending सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि ResponsePending सेट है या नहीं।
### getResume() {#getResume--}
```
public final Date getResume()
```


Resume का मान प्राप्त करता है।

**Returns:**
java.util.Date - Resume का मान।
### getSV() {#getSV--}
```
public final double getSV()
```


एसवी का मान प्राप्त करता है।

**Returns:**
double - SV का मान।
### getStart() {#getStart--}
```
public final Date getStart()
```


स्टार्ट का मान प्राप्त करता है।

**Returns:**
java.util.Date - Start का मान।
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


StartVariance का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Stop का मान प्राप्त करता है।

**Returns:**
java.util.Date - Stop का मान।
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि Summary सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि Summary सेट है या नहीं।
### getTask() {#getTask--}
```
public final Task getTask()
```


वह कार्य जिससे एक संसाधन सौंपा गया है।

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का वह इंस्टेंस प्राप्त करता है जिसमें `TimephasedData` के तत्व होते हैं ([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) क्लास।

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ऑब्जेक्ट को `TimephasedData` के इंस्टेंस के साथ लौटाता है ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) क्लास, जो दिए गए प्रारंभ और समाप्ति तिथियों के भीतर [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) के होते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | समय‑फ़ेज़्ड डेटा की प्रारंभ तिथि। |
| समाप्ति | java.util.Date | समय‑फ़ेज़्ड डेटा की समाप्ति तिथि। |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


निर्दिष्ट [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) के दिए गए प्रारंभ और समाप्ति तिथियों के भीतर `TimephasedData` के इंस्टेंस वाले [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास का इंस्टेंस लौटाता है ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) क्लास।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | समय‑फ़ेज़्ड डेटा की प्रारंभ तिथि। |
| समाप्ति | java.util.Date | समय‑फ़ेज़्ड डेटा की समाप्ति तिथि। |
| timephasedType | byte | समय‑फ़ेज़्ड डेटा का प्रकार ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | तारीख‑समय अंतराल की शुरुआत। |
| समाप्ति | java.util.Date | तारीख‑समय अंतराल का अंत। |

**Returns:**
double - निर्दिष्ट तारीख‑समय अंतराल के लिए समय‑फेज़्ड कार्य की मात्रा।
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | तारीख‑समय अंतराल की शुरुआत। |
| समाप्ति | java.util.Date | तारीख‑समय अंतराल का अंत। |
| timephasedDataType | byte | उपयोग करने के लिए समय‑फेज़्ड डेटा का प्रकार। |

**Returns:**
double - निर्दिष्ट तारीख‑समय अंतराल के लिए समय‑फेज़्ड कार्य की मात्रा।
### getUid() {#getUid--}
```
public final int getUid()
```


यूआईडी का मान प्राप्त करता है।

**Returns:**
int - Uid का मान।
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Units का मान प्राप्त करता है।

**Returns:**
double - Units का मान।
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि UpdateNeeded सेट है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि UpdateNeeded सेट है या नहीं।
### getVAC() {#getVAC--}
```
public final double getVAC()
```


VAC का मान प्राप्त करता है।

**Returns:**
double - VAC का मान।
### getWork() {#getWork--}
```
public final Duration getWork()
```


वर्क का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


WorkContour का मान प्राप्त करता है।

**Returns:**
int - WorkContour का मान।
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


WorkVariance का मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


इस संसाधन असाइनमेंट में बच्चों के होने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - हमेशा गलत।
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


HasFixedRateUnits सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - यह दर्शाने वाला मान कि HasFixedRateUnits सेट है या नहीं।
### hashCode() {#hashCode--}
```
public int hashCode()
```


यह [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास के उदाहरण के लिए हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


समय-फ़ेज़ डेटा की सूची उत्पन्न करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | निर्दिष्ट प्रारंभ तिथि। |
| time | double | निर्दिष्ट कार्य समय। |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | निर्दिष्ट कार्य कैलेंडर। |
| सूची | java.util.List<com.aspose.tasks.TimephasedData> | समय-फ़ेज़्ड डेटा की सूची। |
| isWorking | boolean | निर्दिष्ट फ़्लैग जो बताता है कि समय-फ़ेज़्ड डेटा कार्यशील है या नहीं। |
| प्रकार | int | निर्दिष्ट समय-फ़ेज़्ड डेटा प्रकार। |

**Returns:**
java.util.Date - सूची से अधिकतम तिथि या यदि सूची खाली है तो प्रारंभ तिथि।
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | ACWP का मान। |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | ActualCost का मान। |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


ActualFinish का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | ActualFinish का मान। |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


ActualStart का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | ActualStart का मान। |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Confirmed सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि Confirmed सेट है या नहीं। |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | Cost का मान। |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


CostRateTableType का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | CostRateTableType का मान। |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Delay का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Delay का मान। |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


इस ऑब्जेक्ट के लिए ExtendedAttributeCollection क्लास का एक उदाहरण सेट करता है।

--------------------

केवल XML प्रारूप के लिए पढ़ना समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | इस ऑब्जेक्ट के लिए ExtendedAttributeCollection क्लास का एक उदाहरण। |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Finish का मान। |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


FinishVariance का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | FinishVariance का मान। |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


FixedMaterial सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि FixedMaterial सेट है या नहीं। |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


HasFixedRateUnits सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि HasFixedRateUnits सेट है या नहीं। |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.UUID | इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता। |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Hyperlink का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Hyperlink का मान। |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


HyperlinkAddress का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | HyperlinkAddress का मान। |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


HyperlinkSubAddress का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | HyperlinkSubAddress का मान। |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


LevelingDelay का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | LevelingDelay का मान। |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


LinkedFields सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि LinkedFields सेट है या नहीं। |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


चर सामग्री खपत वाले सामग्री संसाधन के असाइनमेंट के लिए इकाइयों को सेट करता है। चर सामग्री खपत का अर्थ है कि असाइनमेंट अवधि बदलने पर उपयोग की गई सामग्री की मात्रा अनुपातिक रूप से बदलती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| इकाइयाँ | double | समय अवधि में संचित इकाइयों की संख्या। |
|  | rateScaleType | int | समय अवधि जिसमें इकाई मूल्य संचित होता है। |

--------------------

उदाहरण के लिए, '123/माह' सेट करने के लिए, SetUnitsScaled(123D, RateScaleType.Month) को कॉल किया जाना चाहिए। |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Milestone सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि माइलस्टोन सेट है या नहीं। |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


RTF प्रारूप में टेक्स्ट नोट्स सेट करता है।

--------------------

केवल MPP फ़ॉर्मेट्स के लिए समर्थित।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | RTF प्रारूप में पाठ नोट्स। |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


RTF डेटा से निकाले गए नोट्स का साधारण टेक्स्ट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | RTF डेटा से निकाला गया नोट्स का साधारण पाठ। |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Overallocated सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि Overallocated सेट है या नहीं। |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | OvertimeCost का मान। |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


RateScale का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | RateScale का मान। |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


एक कार्य को सौंपा गया संसाधन।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | कार्य को सौंपा गया संसाधन। |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


ResponsePending सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि ResponsePending सेट है या नहीं। |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Resume का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Resume का मान। |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | SV का मान। |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Start का मान। |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


StartVariance का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | StartVariance का मान। |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Stop का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | Stop का मान। |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Summary सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि Summary सेट है या नहीं। |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


वह कार्य जिससे एक संसाधन सौंपा गया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | कार्य जिससे एक संसाधन सौंपा गया है। |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) क्लास की वह इंस्टेंस सेट करता है जिसमें `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) तत्व होते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | क्लास [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) का उदाहरण जिसमें `TimephasedData` के तत्व शामिल हैं ([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) क्लास। |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Uid का मान। |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Units का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | Units का मान। |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


UpdateNeeded सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि UpdateNeeded सेट है या नहीं। |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


VAC का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | VAC का मान। |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work का मान। |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


WorkContour का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | WorkContour का मान। |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


WorkVariance का मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | WorkVariance का मान। |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


टास्क को दो भागों में विभाजित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | विभाजन के आधार पर कार्य व्यवधान की शुरुआत। |
| समाप्ति | java.util.Date | विभाजन के आधार पर कार्य व्यवधान का अंत। |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | विभाजन के आधार पर कैलेंडर। |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


टास्क की अवधि और निर्धारित प्रारंभ तिथि के आधार पर टाइम-फेज़्ड डेटा की सूची उत्पन्न करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | समय-फ़ेज़्ड डेटा उत्पन्न करने के लिए कैलेंडर। |

### toString() {#toString--}
```
public String toString()
```


इंस्टेंस के छोटे स्ट्रिंग प्रतिनिधित्व को लौटाता है [ResourceAssignment](../../com.aspose.tasks/resourceassignment) क्लास का। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं।

**Returns:**
java.lang.String - छोटा स्ट्रिंग जो असाइनमेंट ऑब्जेक्ट का प्रतिनिधित्व करता है।
