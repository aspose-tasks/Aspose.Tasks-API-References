---
title: "Resource"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트의 리소스를 나타냅니다."
type: docs
weight: 248
url: /ko/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

프로젝트의 리소스를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 이 컨테이너에서 속성이 매핑된 값을 반환합니다. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [canLevel()](#canLevel--) | CanLevel이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [delete()](#delete--) | 프로젝트에서 리소스와 해당 할당을 삭제합니다. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | 이 인스턴스가 지정된 [Resource](../../com.aspose.tasks/resource) 클래스의 인스턴스와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getACWP()](#getACWP--) | ACWP 값을 가져옵니다. |
| [getAccrueAt()](#getAccrueAt--) | AccrueAt 값을 가져옵니다. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | ActiveDirectoryGuid 값을 가져옵니다. |
| [getActualCost()](#getActualCost--) | ActualCost 값을 가져옵니다. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost 값을 가져옵니다. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork 값을 가져옵니다. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected 값을 가져옵니다. |
| [getActualWork()](#getActualWork--) | ActualWork 값을 가져옵니다. |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected 값을 가져옵니다. |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner 값을 가져옵니다. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid 값을 가져옵니다. |
| [getAssignments()](#getAssignments--) | 이 객체에 대한 리소스 할당 컬렉션을 가져옵니다. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) 클래스의 인스턴스를 가져옵니다. |
| [getAvailableFrom()](#getAvailableFrom--) | AvailableFrom 값을 가져옵니다. |
| [getAvailableTo()](#getAvailableTo--) | AvailableTo 값을 가져옵니다. |
| [getBCWP()](#getBCWP--) | BCWP 값을 가져옵니다. |
| [getBCWS()](#getBCWS--) | BCWS 값을 가져옵니다. |
| [getBaselines()](#getBaselines--) | 이 객체에 대한 BaselineCollection 인스턴스를 가져옵니다. |
| [getBookingType()](#getBookingType--) | BookingType 값을 가져옵니다. |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost 값을 가져옵니다. |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork 값을 가져옵니다. |
| [getCV()](#getCV--) | CV 값을 가져옵니다. |
| [getCalendar()](#getCalendar--) | Calendar 값을 가져옵니다. |
| [getCode()](#getCode--) | Code의 값을 가져옵니다. |
| [getCost()](#getCost--) | Cost의 값을 가져옵니다. |
| [getCostCenter()](#getCostCenter--) | CostCenter의 값을 가져옵니다. |
| [getCostPerUse()](#getCostPerUse--) | CostPerUse의 값을 가져옵니다. |
| [getCostVariance()](#getCostVariance--) | CostVariance의 값을 가져옵니다. |
| [getCreated()](#getCreated--) | Created의 값을 가져옵니다. |
| [getEMailAddress()](#getEMailAddress--) | EMailAddress의 값을 가져옵니다. |
| [getExtendedAttributes()](#getExtendedAttributes--) | 확장 속성의 값을 가져옵니다. |
| [getFinish()](#getFinish--) | Finish의 값을 가져옵니다. |
| [getGroup()](#getGroup--) | Group의 값을 가져옵니다. |
| [getGuid()](#getGuid--) | Guid의 값을 가져옵니다. |
| [getHyperlink()](#getHyperlink--) | 리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트를 가져옵니다. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | 리소스와 연결된 하이퍼링크의 주소를 가져옵니다. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | 리소스와 연결된 하이퍼링크의 문서 내 특정 위치를 가져옵니다. |
| [getId()](#getId--) | Id의 값을 가져옵니다. |
| [getInactive()](#getInactive--) | Inactive가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getInitials()](#getInitials--) | Initials의 값을 가져옵니다. |
| [getItems()](#getItems--) | 자식 리소스를 가져옵니다. |
| [getMaterialLabel()](#getMaterialLabel--) | MaterialLabel의 값을 가져옵니다. |
| [getMaxUnits()](#getMaxUnits--) | MaxUnits의 값을 가져옵니다. |
| [getName()](#getName--) | Name의 값을 가져옵니다. |
| [getNotesRTF()](#getNotesRTF--) | NotesRTF의 값을 가져옵니다. |
| [getNotesText()](#getNotesText--) | NotesText의 값을 가져옵니다. |
| [getOutlineCode()](#getOutlineCode--) | OutlineCodeCollection 객체를 가져옵니다. |
| [getOverallocated()](#getOverallocated--) | Overallocated가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost의 값을 가져옵니다. |
| [getOvertimeRate()](#getOvertimeRate--) | OvertimeRate의 값을 가져옵니다. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | OvertimeRateFormat의 값을 가져옵니다. |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork의 값을 가져옵니다. |
| [getParentProject()](#getParentProject--) | 이 컨테이너의 상위 프로젝트를 가져옵니다. |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits의 값을 가져옵니다. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete의 값을 가져옵니다. |
| [getPhonetics()](#getPhonetics--) | Phonetics의 값을 가져옵니다. |
| [getRates()](#getRates--) | 이 객체에 대한 [RateCollection](../../com.aspose.tasks/ratecollection) 클래스의 인스턴스를 가져옵니다. |
| [getRegularWork()](#getRegularWork--) | RegularWork의 값을 가져옵니다. |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost의 값을 가져옵니다. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost의 값을 가져옵니다. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork의 값을 가져옵니다. |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork의 값을 가져옵니다. |
| [getSV()](#getSV--) | SV의 값을 가져옵니다. |
| [getStandardRate()](#getStandardRate--) | StandardRate의 값을 가져옵니다. |
| [getStandardRateFormat()](#getStandardRateFormat--) | StandardRateFormat의 값을 가져옵니다. |
| [getStart()](#getStart--) | Start의 값을 가져옵니다. |
| [getTimephasedData()](#getTimephasedData--) | 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 가져옵니다. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | 주어진 시작 및 종료 날짜 내의 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 값을 포함하여 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)를 반환합니다. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | 지정된 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)의 주어진 시작 및 종료 날짜 내의 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimePhasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 값을 포함하여 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 반환합니다. |
| [getType()](#getType--) | Type의 값을 가져옵니다. |
| [getUid()](#getUid--) | Uid의 값을 가져옵니다. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | WindowsUserAccount의 값을 가져옵니다. |
| [getWork()](#getWork--) | Work의 값을 가져옵니다. |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance의 값을 가져옵니다. |
| [getWorkgroup()](#getWorkgroup--) | Workgroup의 값을 가져옵니다. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | [Resource](../../com.aspose.tasks/resource) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [isBudget()](#isBudget--) | IsBudget가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [isCostResource()](#isCostResource--) | IsCostResource가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [isEnterprise()](#isEnterprise--) | IsEnterprise가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [isGeneric()](#isGeneric--) | IsGeneric이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [isNull()](#isNull--) | IsNull이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [isRoot()](#isRoot--) | 리소스가 루트 리소스인지 여부를 나타내는 플래그를 가져옵니다. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [setACWP(double value)](#setACWP-double-) | ACWP의 값을 설정합니다. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | AccrueAt의 값을 설정합니다. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | ActiveDirectoryGuid의 값을 설정합니다. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost의 값을 설정합니다. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost의 값을 설정합니다. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork의 값을 설정합니다. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected의 값을 설정합니다. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork의 값을 설정합니다. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected의 값을 설정합니다. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner의 값을 설정합니다. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid의 값을 설정합니다. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | AvailableFrom의 값을 설정합니다. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | AvailableTo의 값을 설정합니다. |
| [setBCWP(double value)](#setBCWP-double-) | BCWP의 값을 설정합니다. |
| [setBCWS(double value)](#setBCWS-double-) | BCWS의 값을 설정합니다. |
| [setBookingType(int value)](#setBookingType-int-) | BookingType의 값을 설정합니다. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | IsBudget가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost의 값을 설정합니다. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork의 값을 설정합니다. |
| [setCV(double value)](#setCV-double-) | CV의 값을 설정합니다. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar의 값을 설정합니다. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | CanLevel이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setCode(String value)](#setCode-java.lang.String-) | Code의 값을 설정합니다. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost의 값을 설정합니다. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | CostCenter의 값을 설정합니다. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | CostPerUse의 값을 설정합니다. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | IsCostResource가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance의 값을 설정합니다. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created의 값을 설정합니다. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | EMailAddress의 값을 설정합니다. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | IsEnterprise가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish의 값을 설정합니다. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | IsGeneric가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Group의 값을 설정합니다. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Guid의 값을 설정합니다. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | 리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트를 설정합니다. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | 리소스와 연결된 하이퍼링크의 주소를 설정합니다. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | 리소스와 연결된 하이퍼링크의 문서 내 특정 위치를 설정합니다. |
| [setId(int value)](#setId-int-) | Id의 값을 설정합니다. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Inactive가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Initials의 값을 설정합니다. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | MaterialLabel의 값을 설정합니다. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | MaxUnits의 값을 설정합니다. |
| [setName(String value)](#setName-java.lang.String-) | Name의 값을 설정합니다. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | NotesRTF의 값을 설정합니다. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | NotesText의 값을 설정합니다. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | IsNull이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Overallocated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost의 값을 설정합니다. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | OvertimeRate의 값을 설정합니다. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | OvertimeRateFormat의 값을 설정합니다. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork의 값을 설정합니다. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits의 값을 설정합니다. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete의 값을 설정합니다. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Phonetics의 값을 설정합니다. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork의 값을 설정합니다. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost의 값을 설정합니다. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost의 값을 설정합니다. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork의 값을 설정합니다. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork의 값을 설정합니다. |
| [setSV(double value)](#setSV-double-) | SV의 값을 설정합니다. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | StandardRate의 값을 설정합니다. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | StandardRateFormat의 값을 설정합니다. |
| [setStart(Date value)](#setStart-java.util.Date-) | Start의 값을 설정합니다. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 이 객체에 대해 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 설정합니다. |
| [setType(int value)](#setType-int-) | Type의 값을 설정합니다. |
| [setUid(int value)](#setUid-int-) | Uid의 값을 설정합니다. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | WindowsUserAccount의 값을 설정합니다. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work의 값을 설정합니다. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | WorkVariance의 값을 설정합니다. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Workgroup의 값을 설정합니다. |
| [toString()](#toString--) | [Resource](../../com.aspose.tasks/resource) 클래스 인스턴스의 짧은 문자열 표현을 반환합니다. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


이 컨테이너에서 속성이 매핑된 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키입니다. 속성 키를 가져오기 위해 [Rsc](../../com.aspose.tasks/rsc)를 사용합니다. |

**Returns:**
T - 이 컨테이너에서 속성이 매핑되는 값입니다.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키입니다. 속성 키를 가져오기 위해 [Rsc](../../com.aspose.tasks/rsc)를 사용합니다. |
| val | T | 값입니다. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


CanLevel이 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


프로젝트에서 리소스와 해당 할당을 삭제합니다.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


이 인스턴스가 지정된 [Resource](../../com.aspose.tasks/resource) 클래스의 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | 이 인스턴스와 비교할 지정된 [Resource](../../com.aspose.tasks/resource) 클래스 인스턴스입니다. |

**Returns:**
boolean - 지정된 [Resource](../../com.aspose.tasks/resource) 클래스 인스턴스가 이 인스턴스와 동일한 Uid 값을 가지고 있으면 **True**, 그렇지 않으면 **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - 지정된 객체가 이 인스턴스와 동일한 Uid 값을 가진 Resource이면 **True**, 그렇지 않으면 **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP 값을 가져옵니다.

**Returns:**
double - ACWP 값입니다.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


AccrueAt 값을 가져옵니다.

**Returns:**
int - AccrueAt 값입니다.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


ActiveDirectoryGuid 값을 가져옵니다.

**Returns:**
java.lang.String - ActiveDirectoryGuid 값입니다.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - ActualCost 값입니다.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - ActualOvertimeCost 값입니다.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner 값을 가져옵니다.

**Returns:**
java.lang.String - AssignmentOwner 값입니다.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid 값을 가져옵니다.

**Returns:**
java.lang.String - AssignmentOwnerGuid 값입니다.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


이 객체에 대한 리소스 할당 컬렉션을 가져옵니다.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) 클래스의 인스턴스를 가져옵니다. 리소스가 사용 가능한 기간들의 컬렉션입니다.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


AvailableFrom 값을 가져옵니다.

**Returns:**
java.util.Date - AvailableFrom의 값.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


AvailableTo 값을 가져옵니다.

**Returns:**
java.util.Date - AvailableTo의 값.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP 값을 가져옵니다.

**Returns:**
double - BCWP의 값.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS 값을 가져옵니다.

**Returns:**
double - BCWS의 값.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


이 객체에 대한 BaselineCollection 인스턴스를 가져옵니다. 리소스에 대한 기준값.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType 값을 가져옵니다.

**Returns:**
int - BookingType의 값.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - BudgetCost의 값.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV 값을 가져옵니다.

**Returns:**
double - CV의 값.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar 값을 가져옵니다.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Code의 값을 가져옵니다.

**Returns:**
java.lang.String - Code의 값.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - Cost의 값.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


CostCenter의 값을 가져옵니다.

**Returns:**
java.lang.String - CostCenter의 값.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


CostPerUse의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - CostPerUse의 값.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


CostVariance의 값을 가져옵니다.

**Returns:**
double - CostVariance의 값.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Created의 값을 가져옵니다.

**Returns:**
java.util.Date - Created의 값.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


EMailAddress의 값을 가져옵니다.

**Returns:**
java.lang.String - EMailAddress의 값.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


확장 속성의 값을 가져옵니다.

--------------------

두 개의 데이터가 필요합니다 - 고유 ID 또는 필드 ID로 지정되는 확장 속성 테이블에 대한 포인터와, 값 자체로 지정되거나 값 목록에 대한 포인터로 지정되는 값.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish의 값을 가져옵니다.

**Returns:**
java.util.Date - Finish의 값.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Group의 값을 가져옵니다.

**Returns:**
java.lang.String - Group의 값.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Guid의 값을 가져옵니다.

**Returns:**
java.lang.String - Guid의 값.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트를 가져옵니다.

**Returns:**
java.lang.String - 리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


리소스와 연결된 하이퍼링크의 주소를 가져옵니다.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

**Returns:**
java.lang.String - 리소스와 연결된 하이퍼링크의 주소.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


리소스와 연결된 하이퍼링크의 문서 내 특정 위치를 가져옵니다.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

**Returns:**
java.lang.String - 리소스와 연결된 하이퍼링크의 문서 내 특정 위치.
### getId() {#getId--}
```
public final int getId()
```


Id의 값을 가져옵니다.

**Returns:**
int - Id의 값.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Inactive가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Initials의 값을 가져옵니다.

**Returns:**
java.lang.String - Initials의 값.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


자식 리소스를 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - 하위 리소스.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


MaterialLabel의 값을 가져옵니다.

**Returns:**
java.lang.String - MaterialLabel의 값.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


MaxUnits의 값을 가져옵니다.

**Returns:**
double - MaxUnits의 값.
### getName() {#getName--}
```
public final String getName()
```


Name의 값을 가져옵니다.

**Returns:**
java.lang.String - Name의 값.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


NotesRTF의 값을 가져옵니다.

**Returns:**
java.lang.String - NotesRTF의 값.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


NotesText의 값을 가져옵니다.

**Returns:**
java.lang.String - NotesText의 값.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


OutlineCodeCollection 객체를 가져옵니다. 개요 코드의 값.

--------------------

두 개의 데이터가 필요합니다 - FieldID로 지정된 개요 코드 테이블에 대한 포인터와 ValueID 또는 ValueGUID로 지정된 값 목록에 대한 포인터 중 하나에 의해 지정된 값.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Overallocated가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - OvertimeCost의 값.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


OvertimeRate의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - OvertimeRate의 값.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


OvertimeRateFormat의 값을 가져옵니다.

**Returns:**
int - OvertimeRateFormat의 값.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


OvertimeWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


이 컨테이너의 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


PeakUnits의 값을 가져옵니다.

**Returns:**
double - PeakUnits의 값.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


PercentWorkComplete의 값을 가져옵니다.

**Returns:**
int - PercentWorkComplete의 값.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Phonetics의 값을 가져옵니다.

**Returns:**
java.lang.String - Phonetics의 값.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


이 객체에 대한 [RateCollection](../../com.aspose.tasks/ratecollection) 클래스의 인스턴스를 가져옵니다. 각 항목과 연관된 기간 및 요율의 컬렉션입니다.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


RegularWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


RemainingCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - RemainingCost의 값.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


RemainingOvertimeCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost의 값.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


RemainingOvertimeWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


RemainingWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


SV의 값을 가져옵니다.

**Returns:**
double - SV의 값.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


StandardRate의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - StandardRate의 값.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


StandardRateFormat의 값을 가져옵니다.

**Returns:**
int - StandardRateFormat의 값.
### getStart() {#getStart--}
```
public final Date getStart()
```


Start의 값을 가져옵니다.

**Returns:**
java.util.Date - Start의 값.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 가져옵니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


주어진 시작 및 종료 날짜 내의 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 값을 포함하여 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시간 구간 데이터의 시작 날짜. |
| 끝 | java.util.Date | 시간 구간 데이터의 종료 날짜. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


지정된 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)의 주어진 시작 및 종료 날짜 내의 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimePhasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 값을 포함하여 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시간 구간 데이터의 시작 날짜. |
| 끝 | java.util.Date | 시간 구간 데이터의 종료 날짜. |
| timephasedType | byte | 시간 구간 데이터의 유형 ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Type의 값을 가져옵니다.

**Returns:**
int - Type의 값.
### getUid() {#getUid--}
```
public final int getUid()
```


Uid의 값을 가져옵니다.

**Returns:**
int - Uid의 값.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


WindowsUserAccount의 값을 가져옵니다.

**Returns:**
java.lang.String - WindowsUserAccount의 값.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


WorkVariance의 값을 가져옵니다.

**Returns:**
double - WorkVariance의 값.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Workgroup의 값을 가져옵니다.

**Returns:**
int - Workgroup의 값.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


내부 사용을 위해 예약됨.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


[Resource](../../com.aspose.tasks/resource) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


IsBudget가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


IsCostResource가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


IsEnterprise가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


IsGeneric이 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


IsNull이 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


리소스가 루트 리소스인지 여부를 나타내는 플래그를 가져옵니다. 루트 리소스는 MS Project 형식의 내부를 지원하도록 설계된 특수 리소스로, 사용자의 코드에서 직접 사용하도록 의도되지 않았습니다.

**Returns:**
boolean - 리소스가 루트 리소스인지 여부를 나타내는 플래그.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | 지정된 속성 키입니다. 속성 키를 가져오기 위해 [Rsc](../../com.aspose.tasks/rsc)를 사용합니다. |
| val | java.util.Date | 값입니다. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | ACWP의 값. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


AccrueAt의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | AccrueAt의 값. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


ActiveDirectoryGuid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | ActiveDirectoryGuid의 값. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | ActualCost의 값. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | ActualOvertimeCost의 값. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork의 값. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected의 값. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork의 값. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected의 값. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | AssignmentOwner의 값. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | AssignmentOwnerGuid의 값. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


AvailableFrom의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | AvailableFrom의 값. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


AvailableTo의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | AvailableTo의 값. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | BCWP의 값. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | BCWS의 값. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | BookingType의 값. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


IsBudget가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsBudget가 설정되어 있는지 여부를 나타내는 값. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | BudgetCost의 값. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork의 값. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | CV의 값. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Calendar의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | Calendar의 값. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


CanLevel이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | CanLevel가 설정되어 있는지 여부를 나타내는 값. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Code의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Code의 값. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | Cost의 값. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


CostCenter의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | CostCenter의 값. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


CostPerUse의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | CostPerUse의 값. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


IsCostResource가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsCostResource가 설정되어 있는지 여부를 나타내는 값. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | CostVariance의 값. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Created의 값. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


EMailAddress의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | EMailAddress의 값. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


IsEnterprise가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsEnterprise가 설정되어 있는지 여부를 나타내는 값. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Finish의 값. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


IsGeneric가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsGeneric가 설정되어 있는지 여부를 나타내는 값. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Group의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Group의 값. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Guid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Guid의 값. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 리소스와 연결된 하이퍼링크의 제목 또는 설명 텍스트. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


리소스와 연결된 하이퍼링크의 주소를 설정합니다.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 리소스와 연결된 하이퍼링크의 주소. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


리소스와 연결된 하이퍼링크의 문서 내 특정 위치를 설정합니다.

--------------------

하이퍼링크의 전체 주소(Microsoft Project의 Hyperlink Href)는 HyperlinkAddress와 HyperlinkSubAddress를 연결한 것입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 리소스와 연결된 하이퍼링크의 문서 내 특정 위치. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Id의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Id 값. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Inactive가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Inactive가 설정되었는지 여부를 나타내는 값. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Initials의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Initials 값. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


MaterialLabel의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | MaterialLabel 값. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


MaxUnits의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | MaxUnits 값. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Name의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Name 값. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


NotesRTF의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | NotesRTF 값. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


NotesText의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | NotesText 값. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


IsNull이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsNull이 설정되었는지 여부를 나타내는 값. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Overallocated가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Overallocated가 설정되었는지 여부를 나타내는 값. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | OvertimeCost 값. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


OvertimeRate의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | OvertimeRate 값. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


OvertimeRateFormat의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | OvertimeRateFormat 값. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork 값. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | PeakUnits 값. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | PercentWorkComplete 값. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Phonetics의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Phonetics 값. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork 값. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | RemainingCost 값. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | RemainingOvertimeCost 값. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork 값. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork 값. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | SV 값. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


StandardRate의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | StandardRate의 값. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


StandardRateFormat의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | StandardRateFormat의 값. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Start의 값. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | IsTeamAssignmentPool이 설정되었는지 여부를 나타내는 값. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


이 객체에 대해 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 설정합니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Type의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Type의 값. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Uid의 값. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


WindowsUserAccount의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | WindowsUserAccount의 값. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work의 값. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


WorkVariance의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | WorkVariance의 값. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Workgroup의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Workgroup의 값. |

### toString() {#toString--}
```
public String toString()
```


리소스 클래스의 인스턴스인 [Resource](../../com.aspose.tasks/resource)의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다.

**Returns:**
java.lang.String - 리소스 객체를 나타내는 짧은 문자열.
