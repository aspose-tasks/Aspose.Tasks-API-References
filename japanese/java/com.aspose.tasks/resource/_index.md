---
title: "Resource"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト内のリソースを表します。"
type: docs
weight: 248
url: /ja/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

プロジェクト内のリソースを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | このコンテナ内でプロパティがマッピングされている値を返します。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | このコンテナ内で指定されたプロパティを指定された値にマッピングします。 |
| [canLevel()](#canLevel--) | CanLevel が設定されているかどうかを示す値を取得します。 |
| [delete()](#delete--) | プロジェクトからリソースとその割り当てを削除します。 |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | このインスタンスが指定された [Resource](../../com.aspose.tasks/resource) クラスのインスタンスと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getACWP()](#getACWP--) | ACWP の値を取得します。 |
| [getAccrueAt()](#getAccrueAt--) | AccrueAt の値を取得します。 |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | ActiveDirectoryGuid の値を取得します。 |
| [getActualCost()](#getActualCost--) | ActualCost の値を取得します。 |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost の値を取得します。 |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork の値を取得します。 |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected の値を取得します。 |
| [getActualWork()](#getActualWork--) | ActualWork の値を取得します。 |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected の値を取得します。 |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner の値を取得します。 |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid の値を取得します。 |
| [getAssignments()](#getAssignments--) | このオブジェクトのリソース割り当てコレクションを取得します。 |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | このオブジェクトの [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) クラスのインスタンスを取得します。 |
| [getAvailableFrom()](#getAvailableFrom--) | AvailableFrom の値を取得します。 |
| [getAvailableTo()](#getAvailableTo--) | AvailableTo の値を取得します。 |
| [getBCWP()](#getBCWP--) | BCWP の値を取得します。 |
| [getBCWS()](#getBCWS--) | BCWS の値を取得します。 |
| [getBaselines()](#getBaselines--) | このオブジェクトの BaselineCollection インスタンスを取得します。 |
| [getBookingType()](#getBookingType--) | BookingType の値を取得します。 |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost の値を取得します。 |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork の値を取得します。 |
| [getCV()](#getCV--) | CV の値を取得します。 |
| [getCalendar()](#getCalendar--) | Calendar の値を取得します。 |
| [getCode()](#getCode--) | Code の値を取得します。 |
| [getCost()](#getCost--) | Cost の値を取得します。 |
| [getCostCenter()](#getCostCenter--) | CostCenter の値を取得します。 |
| [getCostPerUse()](#getCostPerUse--) | CostPerUse の値を取得します。 |
| [getCostVariance()](#getCostVariance--) | CostVariance の値を取得します。 |
| [getCreated()](#getCreated--) | Created の値を取得します。 |
| [getEMailAddress()](#getEMailAddress--) | EMailAddress の値を取得します。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | 拡張属性の値を取得します。 |
| [getFinish()](#getFinish--) | Finish の値を取得します。 |
| [getGroup()](#getGroup--) | Group の値を取得します。 |
| [getGuid()](#getGuid--) | Guid の値を取得します。 |
| [getHyperlink()](#getHyperlink--) | リソースに関連付けられたハイパーリンクのタイトルまたは説明テキストを取得します。 |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | リソースに関連付けられたハイパーリンクのアドレスを取得します。 |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | リソースに関連付けられたハイパーリンクのドキュメント内の特定の位置を取得します。 |
| [getId()](#getId--) | Id の値を取得します。 |
| [getInactive()](#getInactive--) | Inactive が設定されているかどうかを示す値を取得します。 |
| [getInitials()](#getInitials--) | Initials の値を取得します。 |
| [getItems()](#getItems--) | 子リソースを取得します。 |
| [getMaterialLabel()](#getMaterialLabel--) | MaterialLabel の値を取得します。 |
| [getMaxUnits()](#getMaxUnits--) | MaxUnits の値を取得します。 |
| [getName()](#getName--) | Name の値を取得します。 |
| [getNotesRTF()](#getNotesRTF--) | NotesRTF の値を取得します。 |
| [getNotesText()](#getNotesText--) | NotesText の値を取得します。 |
| [getOutlineCode()](#getOutlineCode--) | OutlineCodeCollection オブジェクトを取得します。 |
| [getOverallocated()](#getOverallocated--) | Overallocated が設定されているかどうかを示す値を取得します。 |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost の値を取得します。 |
| [getOvertimeRate()](#getOvertimeRate--) | OvertimeRate の値を取得します。 |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | OvertimeRateFormat の値を取得します。 |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork の値を取得します。 |
| [getParentProject()](#getParentProject--) | このコンテナの親プロジェクトを取得します。 |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits の値を取得します。 |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete の値を取得します。 |
| [getPhonetics()](#getPhonetics--) | Phonetics の値を取得します。 |
| [getRates()](#getRates--) | このオブジェクトの [RateCollection](../../com.aspose.tasks/ratecollection) クラスのインスタンスを取得します。 |
| [getRegularWork()](#getRegularWork--) | RegularWork の値を取得します。 |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost の値を取得します。 |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost の値を取得します。 |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork の値を取得します。 |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork の値を取得します。 |
| [getSV()](#getSV--) | SV の値を取得します。 |
| [getStandardRate()](#getStandardRate--) | StandardRate の値を取得します。 |
| [getStandardRateFormat()](#getStandardRateFormat--) | StandardRateFormat の値を取得します。 |
| [getStart()](#getStart--) | Start の値を取得します。 |
| [getTimephasedData()](#getTimephasedData--) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを取得します。 |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) を返します。`TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) の値は、指定された開始日と終了日の範囲内です。 |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを返します。`TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimePhasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) の値は、指定された [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) の開始日と終了日の範囲内です。 |
| [getType()](#getType--) | Type の値を取得します。 |
| [getUid()](#getUid--) | Uid の値を取得します。 |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | WindowsUserAccount の値を取得します。 |
| [getWork()](#getWork--) | Work の値を取得します。 |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance の値を取得します。 |
| [getWorkgroup()](#getWorkgroup--) | Workgroup の値を取得します。 |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | インスタンスの [Resource](../../com.aspose.tasks/resource) クラスのハッシュコード値を返します。 |
| [isBudget()](#isBudget--) | IsBudget が設定されているかどうかを示す値を取得します。 |
| [isCostResource()](#isCostResource--) | IsCostResource が設定されているかどうかを示す値を取得します。 |
| [isEnterprise()](#isEnterprise--) | IsEnterprise が設定されているかどうかを示す値を取得します。 |
| [isGeneric()](#isGeneric--) | IsGeneric が設定されているかどうかを示す値を取得します。 |
| [isNull()](#isNull--) | IsNull が設定されているかどうかを示す値を取得します。 |
| [isRoot()](#isRoot--) | リソースがルートリソースかどうかを示すフラグを取得します。 |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | IsTeamAssignmentPool が設定されているかどうかを示す値を取得します。 |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | このコンテナ内で指定されたプロパティを指定された値にマッピングします。 |
| [setACWP(double value)](#setACWP-double-) | ACWP の値を設定します。 |
| [setAccrueAt(int value)](#setAccrueAt-int-) | AccrueAt の値を設定します。 |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | ActiveDirectoryGuid の値を設定します。 |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost の値を設定します。 |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost の値を設定します。 |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork の値を設定します。 |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected の値を設定します。 |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork の値を設定します。 |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected の値を設定します。 |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner の値を設定します。 |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid の値を設定します。 |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | AvailableFrom の値を設定します。 |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | AvailableTo の値を設定します。 |
| [setBCWP(double value)](#setBCWP-double-) | BCWP の値を設定します。 |
| [setBCWS(double value)](#setBCWS-double-) | BCWS の値を設定します。 |
| [setBookingType(int value)](#setBookingType-int-) | BookingType の値を設定します。 |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | IsBudget が設定されているかどうかを示す値を設定します。 |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost の値を設定します。 |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork の値を設定します。 |
| [setCV(double value)](#setCV-double-) | CV の値を設定します。 |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar の値を設定します。 |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | CanLevel が設定されているかどうかを示す値を設定します。 |
| [setCode(String value)](#setCode-java.lang.String-) | Code の値を設定します。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost の値を設定します。 |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | CostCenter の値を設定します。 |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | CostPerUse の値を設定します。 |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | IsCostResource が設定されているかどうかを示す値を設定します。 |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance の値を設定します。 |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created の値を設定します。 |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | EMailAddress の値を設定します。 |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | IsEnterprise が設定されているかどうかを示す値を設定します。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish の値を設定します。 |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | IsGeneric が設定されているかどうかを示す値を設定します。 |
| [setGroup(String value)](#setGroup-java.lang.String-) | Group の値を設定します。 |
| [setGuid(String value)](#setGuid-java.lang.String-) | Guid の値を設定します。 |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | リソースに関連付けられたハイパーリンクのタイトルまたは説明テキストを設定します。 |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | リソースに関連付けられたハイパーリンクのアドレスを設定します。 |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | リソースに関連付けられたハイパーリンクのドキュメント内の特定の場所を設定します。 |
| [setId(int value)](#setId-int-) | Id の値を設定します。 |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Inactive が設定されているかどうかを示す値を設定します。 |
| [setInitials(String value)](#setInitials-java.lang.String-) | Initials の値を設定します。 |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | MaterialLabel の値を設定します。 |
| [setMaxUnits(double value)](#setMaxUnits-double-) | MaxUnits の値を設定します。 |
| [setName(String value)](#setName-java.lang.String-) | Name の値を設定します。 |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | NotesRTF の値を設定します。 |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | NotesText の値を設定します。 |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | IsNull が設定されているかどうかを示す値を設定します。 |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Overallocated が設定されているかどうかを示す値を設定します。 |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost の値を設定します。 |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | OvertimeRate の値を設定します。 |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | OvertimeRateFormat の値を設定します。 |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork の値を設定します。 |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits の値を設定します。 |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete の値を設定します。 |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Phonetics の値を設定します。 |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork の値を設定します。 |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost の値を設定します。 |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost の値を設定します。 |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork の値を設定します。 |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork の値を設定します。 |
| [setSV(double value)](#setSV-double-) | SV の値を設定します。 |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | StandardRate の値を設定します。 |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | StandardRateFormat の値を設定します。 |
| [setStart(Date value)](#setStart-java.util.Date-) | Start の値を設定します。 |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | IsTeamAssignmentPool が設定されているかどうかを示す値を設定します。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | このオブジェクトのために [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを設定します。 |
| [setType(int value)](#setType-int-) | Type の値を設定します。 |
| [setUid(int value)](#setUid-int-) | Uid の値を設定します。 |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | WindowsUserAccount の値を設定します。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work の値を設定します。 |
| [setWorkVariance(double value)](#setWorkVariance-double-) | WorkVariance の値を設定します。 |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Workgroup の値を設定します。 |
| [toString()](#toString--) | [Resource](../../com.aspose.tasks/resource) クラスのインスタンスの短い文字列表現を返します。 |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


このコンテナ内でプロパティがマッピングされている値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティキーです。プロパティキーを取得するには [Rsc](../../com.aspose.tasks/rsc) を使用します。 |

**Returns:**
T - このコンテナ内でプロパティがマッピングされる値です。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


このコンテナ内で指定されたプロパティを指定された値にマッピングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティキーです。プロパティキーを取得するには [Rsc](../../com.aspose.tasks/rsc) を使用します。 |
| val | T | 値です。 |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


CanLevel が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


プロジェクトからリソースとその割り当てを削除します。

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


このインスタンスが指定された [Resource](../../com.aspose.tasks/resource) クラスのインスタンスと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | このインスタンスと比較するための、指定された [Resource](../../com.aspose.tasks/resource) クラスのインスタンスです。 |

**Returns:**
boolean - 指定された [Resource](../../com.aspose.tasks/resource) クラスのインスタンスがこのインスタンスと同じ Uid 値を持つ場合は **True**、それ以外の場合は **false** です。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - 指定されたオブジェクトがこのインスタンスと同じ Uid 値を持つ Resource の場合は **True**、それ以外の場合は **false** です。
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP の値を取得します。

**Returns:**
double - ACWP の値です。
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


AccrueAt の値を取得します。

**Returns:**
int - AccrueAt の値です。
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


ActiveDirectoryGuid の値を取得します。

**Returns:**
java.lang.String - ActiveDirectoryGuid の値です。
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost の値を取得します。

**Returns:**
java.math.BigDecimal - ActualCost の値です。
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - ActualOvertimeCost の値です。
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner の値を取得します。

**Returns:**
java.lang.String - AssignmentOwner の値です。
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid の値を取得します。

**Returns:**
java.lang.String - AssignmentOwnerGuid の値です。
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


このオブジェクトのリソース割り当てコレクションを取得します。

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) クラスのインスタンスを取得します。リソースが利用可能な期間のコレクションです。

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


AvailableFrom の値を取得します。

**Returns:**
java.util.Date - AvailableFrom の値。
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


AvailableTo の値を取得します。

**Returns:**
java.util.Date - AvailableTo の値。
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP の値を取得します。

**Returns:**
double - BCWP の値。
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS の値を取得します。

**Returns:**
double - BCWS の値。
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


このオブジェクトの BaselineCollection インスタンスを取得します。リソースのベースライン値。

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType の値を取得します。

**Returns:**
int - BookingType の値。
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost の値を取得します。

**Returns:**
java.math.BigDecimal - BudgetCost の値。
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV の値を取得します。

**Returns:**
double - CV の値。
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar の値を取得します。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Code の値を取得します。

**Returns:**
java.lang.String - Code の値。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost の値を取得します。

**Returns:**
java.math.BigDecimal - Cost の値。
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


CostCenter の値を取得します。

**Returns:**
java.lang.String - CostCenter の値。
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


CostPerUse の値を取得します。

**Returns:**
java.math.BigDecimal - CostPerUse の値。
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


CostVariance の値を取得します。

**Returns:**
double - CostVariance の値。
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Created の値を取得します。

**Returns:**
java.util.Date - Created の値。
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


EMailAddress の値を取得します。

**Returns:**
java.lang.String - EMailAddress の値。
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


拡張属性の値を取得します。

--------------------

必要なデータは2つです - ユニーク ID または Field ID のいずれかで指定される拡張属性テーブルへのポインタ、そして値は値自体で指定するか、値リストへのポインタのいずれかです。

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish の値を取得します。

**Returns:**
java.util.Date - Finish の値。
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Group の値を取得します。

**Returns:**
java.lang.String - Group の値。
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Guid の値を取得します。

**Returns:**
java.lang.String - Guid の値。
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


リソースに関連付けられたハイパーリンクのタイトルまたは説明テキストを取得します。

**Returns:**
java.lang.String - リソースに関連付けられたハイパーリンクのタイトルまたは説明テキスト。
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


リソースに関連付けられたハイパーリンクのアドレスを取得します。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

**Returns:**
java.lang.String - リソースに関連付けられたハイパーリンクのアドレス。
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


リソースに関連付けられたハイパーリンクのドキュメント内の特定の位置を取得します。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

**Returns:**
java.lang.String - リソースに関連付けられたハイパーリンク内のドキュメントの特定の場所。
### getId() {#getId--}
```
public final int getId()
```


Id の値を取得します。

**Returns:**
int - Id の値。
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Inactive が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Initials の値を取得します。

**Returns:**
java.lang.String - Initials の値。
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


子リソースを取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - 子リソース。
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


MaterialLabel の値を取得します。

**Returns:**
java.lang.String - MaterialLabel の値。
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


MaxUnits の値を取得します。

**Returns:**
double - MaxUnits の値。
### getName() {#getName--}
```
public final String getName()
```


Name の値を取得します。

**Returns:**
java.lang.String - Name の値。
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


NotesRTF の値を取得します。

**Returns:**
java.lang.String - NotesRTF の値。
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


NotesText の値を取得します。

**Returns:**
java.lang.String - NotesText の値。
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


OutlineCodeCollection オブジェクトを取得します。アウトラインコードの値。

--------------------

2 つのデータが必要です - FieldID で指定されたアウトラインコードテーブルへのポインタと、ValueID または ValueGUID によって指定された値リストへのポインタです。

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Overallocated が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - OvertimeCost の値。
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


OvertimeRate の値を取得します。

**Returns:**
java.math.BigDecimal - OvertimeRate の値。
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


OvertimeRateFormat の値を取得します。

**Returns:**
int - OvertimeRateFormat の値。
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


OvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


このコンテナの親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


PeakUnits の値を取得します。

**Returns:**
double - PeakUnits の値。
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


PercentWorkComplete の値を取得します。

**Returns:**
int - PercentWorkComplete の値。
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Phonetics の値を取得します。

**Returns:**
java.lang.String - Phonetics の値。
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


[RateCollection](../../com.aspose.tasks/ratecollection) クラスのインスタンスを取得します。このオブジェクトに関連付けられた期間とレートのコレクションです。

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


RegularWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


RemainingCost の値を取得します。

**Returns:**
java.math.BigDecimal - RemainingCost の値。
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


RemainingOvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost の値。
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


RemainingOvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


RemainingWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


SV の値を取得します。

**Returns:**
double - SV の値。
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


StandardRate の値を取得します。

**Returns:**
java.math.BigDecimal - StandardRate の値。
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


StandardRateFormat の値を取得します。

**Returns:**
int - StandardRateFormat の値。
### getStart() {#getStart--}
```
public final Date getStart()
```


Start の値を取得します。

**Returns:**
java.util.Date - Start の値。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを取得します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) を返します。`TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) の値は、指定された開始日と終了日の範囲内です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 時間分割データの開始日。 |
| 終了 | java.util.Date | 時間分割データの終了日。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを返します。`TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimePhasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) の値は、指定された [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) の開始日と終了日の範囲内です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 時間分割データの開始日。 |
| 終了 | java.util.Date | 時間分割データの終了日。 |
| timephasedType | byte | 時間分割データの種類（[TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)）。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Type の値を取得します。

**Returns:**
int - Type の値。
### getUid() {#getUid--}
```
public final int getUid()
```


Uid の値を取得します。

**Returns:**
int - Uid の値。
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


WindowsUserAccount の値を取得します。

**Returns:**
java.lang.String - WindowsUserAccount の値。
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


WorkVariance の値を取得します。

**Returns:**
double - WorkVariance の値。
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Workgroup の値を取得します。

**Returns:**
int - Workgroup の値。
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


内部使用のために予約されています。

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


インスタンスの [Resource](../../com.aspose.tasks/resource) クラスのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


IsBudget が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


IsCostResource が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


IsEnterprise が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


IsGeneric が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


IsNull が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


リソースがルートリソースかどうかを示すフラグを取得します。ルートリソースは、MS Project のフォーマット内部をサポートするための特別なリソースであり、ユーザーのコードから直接使用することは想定されていません。

**Returns:**
boolean - リソースがルートリソースかどうかを示すフラグ。
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


IsTeamAssignmentPool が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - IsTeamAssignmentPool が設定されているかどうかを示す値。
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


このコンテナ内で指定されたプロパティを指定された値にマッピングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | 指定されたプロパティキーです。プロパティキーを取得するには [Rsc](../../com.aspose.tasks/rsc) を使用します。 |
| val | java.util.Date | 値です。 |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ACWP の値。 |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


AccrueAt の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | AccrueAt の値。 |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


ActiveDirectoryGuid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | ActiveDirectoryGuid の値。 |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | ActualCost の値。 |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | ActualOvertimeCost の値。 |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork の値。 |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected の値。 |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork の値。 |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected の値。 |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | AssignmentOwner の値。 |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | AssignmentOwnerGuid の値。 |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


AvailableFrom の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | AvailableFrom の値。 |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


AvailableTo の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | AvailableTo の値。 |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | BCWP の値。 |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | BCWS の値。 |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | BookingType の値。 |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


IsBudget が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsBudget が設定されているかどうかを示す値。 |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | BudgetCost の値。 |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork の値。 |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | CV の値。 |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Calendar の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | Calendar の値。 |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


CanLevel が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | CanLevel が設定されているかどうかを示す値。 |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Code の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Code の値。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | Cost の値。 |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


CostCenter の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | CostCenter の値。 |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


CostPerUse の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | CostPerUse の値。 |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


IsCostResource が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsCostResource が設定されているかどうかを示す値。 |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | CostVariance の値。 |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Created の値。 |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


EMailAddress の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | EMailAddress の値。 |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


IsEnterprise が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsEnterprise が設定されているかどうかを示す値。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Finish の値。 |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


IsGeneric が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsGeneric が設定されているかどうかを示す値。 |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Group の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Group の値。 |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Guid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Guid の値。 |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


リソースに関連付けられたハイパーリンクのタイトルまたは説明テキストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | リソースに関連付けられたハイパーリンクのタイトルまたは説明テキスト。 |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


リソースに関連付けられたハイパーリンクのアドレスを設定します。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | リソースに関連付けられたハイパーリンクのアドレス。 |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


リソースに関連付けられたハイパーリンクのドキュメント内の特定の場所を設定します。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | リソースに関連付けられたハイパーリンク内のドキュメントの特定の場所。 |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Id の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Id の値。 |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Inactive が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Inactive が設定されているかどうかを示す値。 |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Initials の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Initials の値。 |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


MaterialLabel の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | MaterialLabel の値。 |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


MaxUnits の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | MaxUnits の値。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Name の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Name の値。 |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


NotesRTF の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | NotesRTF の値。 |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


NotesText の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | NotesText の値。 |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


IsNull が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsNull が設定されているかどうかを示す値。 |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Overallocated が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Overallocated が設定されているかどうかを示す値。 |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | OvertimeCost の値。 |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


OvertimeRate の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | OvertimeRate の値。 |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


OvertimeRateFormat の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | OvertimeRateFormat の値。 |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork の値。 |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | PeakUnits の値。 |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | PercentWorkComplete の値。 |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Phonetics の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Phonetics の値。 |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork の値。 |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | RemainingCost の値。 |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | RemainingOvertimeCost の値。 |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork の値。 |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork の値。 |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | SV の値。 |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


StandardRate の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | StandardRate の値。 |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


StandardRateFormat の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | StandardRateFormat の値。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Start の値。 |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


IsTeamAssignmentPool が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | IsTeamAssignmentPool が設定されているかどうかを示す値。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


このオブジェクトのために [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを設定します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンス。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Type の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Type の値。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Uid の値。 |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


WindowsUserAccount の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | WindowsUserAccount の値。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work の値。 |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


WorkVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | WorkVariance の値。 |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Workgroup の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Workgroup の値。 |

### toString() {#toString--}
```
public String toString()
```


[Resource](../../com.aspose.tasks/resource) クラスのインスタンスの短い文字列表現を返します。表現の正確な詳細は未定義で、変更される可能性があります。

**Returns:**
java.lang.String - リソースオブジェクトを表す短い文字列。
