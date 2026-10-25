---
title: "Resource"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un recurso en un proyecto."
type: docs
weight: 248
url: /es/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Representa un recurso en un proyecto.
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Devuelve el valor al que la propiedad está mapeada en este contenedor. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [canLevel()](#canLevel--) | Obtiene un valor que indica si CanLevel está establecido o no. |
| [delete()](#delete--) | Elimina un recurso y sus asignaciones del proyecto. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getACWP()](#getACWP--) | Obtiene un valor de ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Obtiene un valor de AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Obtiene un valor de ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Obtiene un valor de ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Obtiene un valor de ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Obtiene un valor de ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Obtiene un valor de ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Obtiene un valor de ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Obtiene un valor de ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Obtiene un valor de AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Obtiene un valor de AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Obtiene una colección de asignaciones de recursos para este objeto. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Obtiene la instancia de la clase [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Obtiene un valor de AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Obtiene un valor de AvailableTo. |
| [getBCWP()](#getBCWP--) | Obtiene un valor de BCWP. |
| [getBCWS()](#getBCWS--) | Obtiene un valor de BCWS. |
| [getBaselines()](#getBaselines--) | Obtiene una instancia de BaselineCollection para este objeto. |
| [getBookingType()](#getBookingType--) | Obtiene un valor de BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Obtiene un valor de BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Obtiene un valor de BudgetWork. |
| [getCV()](#getCV--) | Obtiene un valor de CV. |
| [getCalendar()](#getCalendar--) | Obtiene un valor de Calendar. |
| [getCode()](#getCode--) | Obtiene un valor de Code. |
| [getCost()](#getCost--) | Obtiene un valor de Cost. |
| [getCostCenter()](#getCostCenter--) | Obtiene un valor de CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Obtiene un valor de CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Obtiene un valor de CostVariance. |
| [getCreated()](#getCreated--) | Obtiene un valor de Created. |
| [getEMailAddress()](#getEMailAddress--) | Obtiene un valor de EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtiene los valores de un atributo extendido. |
| [getFinish()](#getFinish--) | Obtiene un valor de Finish. |
| [getGroup()](#getGroup--) | Obtiene un valor de Group. |
| [getGuid()](#getGuid--) | Obtiene un valor de Guid. |
| [getHyperlink()](#getHyperlink--) | Obtiene el título o texto explicativo de un hipervínculo asociado a un recurso. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Obtiene la dirección de un hipervínculo asociado a un recurso. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Obtiene la ubicación específica en un documento de un hipervínculo asociado a un recurso. |
| [getId()](#getId--) | Obtiene un valor de Id. |
| [getInactive()](#getInactive--) | Obtiene un valor que indica si Inactive está establecido o no. |
| [getInitials()](#getInitials--) | Obtiene un valor de Initials. |
| [getItems()](#getItems--) | Obtiene recursos hijos. |
| [getMaterialLabel()](#getMaterialLabel--) | Obtiene un valor de MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Obtiene un valor de MaxUnits. |
| [getName()](#getName--) | Obtiene un valor de Name. |
| [getNotesRTF()](#getNotesRTF--) | Obtiene un valor de NotesRTF. |
| [getNotesText()](#getNotesText--) | Obtiene un valor de NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Obtiene un objeto OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | Obtiene un valor que indica si Overallocated está establecido o no. |
| [getOvertimeCost()](#getOvertimeCost--) | Obtiene un valor de OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Obtiene un valor de OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Obtiene un valor de OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Obtiene un valor de OvertimeWork. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto principal para este contenedor. |
| [getPeakUnits()](#getPeakUnits--) | Obtiene un valor de PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Obtiene un valor de PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Obtiene un valor de Phonetics. |
| [getRates()](#getRates--) | Obtiene la instancia de la clase [RateCollection](../../com.aspose.tasks/ratecollection) para este objeto. |
| [getRegularWork()](#getRegularWork--) | Obtiene un valor de RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Obtiene un valor de RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Obtiene un valor de RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Obtiene un valor de RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Obtiene un valor de RemainingWork. |
| [getSV()](#getSV--) | Obtiene un valor de SV. |
| [getStandardRate()](#getStandardRate--) | Obtiene un valor de StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Obtiene un valor de StandardRateFormat. |
| [getStart()](#getStart--) | Obtiene un valor de Start. |
| [getTimephasedData()](#getTimephasedData--) | Obtiene una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Devuelve [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto con los valores de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dentro de las fechas de inicio y fin proporcionadas. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Devuelve una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto con los valores de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dentro de las fechas de inicio y fin proporcionadas del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) especificado. |
| [getType()](#getType--) | Obtiene un valor de Type. |
| [getUid()](#getUid--) | Obtiene un valor de Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Obtiene un valor de WindowsUserAccount. |
| [getWork()](#getWork--) | Obtiene un valor de Work. |
| [getWorkVariance()](#getWorkVariance--) | Obtiene un valor de WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Obtiene un valor de Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Obtiene un valor que indica si IsBudget está establecido o no. |
| [isCostResource()](#isCostResource--) | Obtiene un valor que indica si IsCostResource está establecido o no. |
| [isEnterprise()](#isEnterprise--) | Obtiene un valor que indica si IsEnterprise está establecido o no. |
| [isGeneric()](#isGeneric--) | Obtiene un valor que indica si IsGeneric está establecido o no. |
| [isNull()](#isNull--) | Obtiene un valor que indica si IsNull está establecido o no. |
| [isRoot()](#isRoot--) | Obtiene la bandera que indica si el recurso es un recurso raíz. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Obtiene un valor que indica si IsTeamAssignmentPool está establecido o no. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [setACWP(double value)](#setACWP-double-) | Establece un valor de ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Establece un valor de AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Establece un valor de ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Establece un valor de ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Establece un valor de ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Establece un valor de ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Establece un valor de ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Establece un valor de ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Establece un valor de AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Establece un valor de AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Establece un valor de AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Establece un valor de AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Establece un valor de BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Establece un valor de BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Establece un valor de BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Establece un valor que indica si IsBudget está establecido o no. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Establece un valor de BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Establece un valor de BudgetWork. |
| [setCV(double value)](#setCV-double-) | Establece un valor de CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Establece un valor de Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Establece un valor que indica si CanLevel está establecido o no. |
| [setCode(String value)](#setCode-java.lang.String-) | Establece un valor de Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Establece un valor de Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Establece un valor de CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Establece un valor de CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Establece un valor que indica si IsCostResource está establecido o no. |
| [setCostVariance(double value)](#setCostVariance-double-) | Establece un valor de CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Establece un valor de Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Establece un valor de EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Establece un valor que indica si IsEnterprise está establecido o no. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Establece un valor de Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Establece un valor que indica si IsGeneric está establecido o no. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Establece un valor de Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Establece un valor de Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Establece el título o texto explicativo de un hipervínculo asociado a un recurso. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Establece la dirección de un hipervínculo asociado a un recurso. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Establece la ubicación específica en un documento en un hipervínculo asociado a un recurso. |
| [setId(int value)](#setId-int-) | Establece un valor de Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Establece un valor que indica si Inactive está establecido o no. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Establece un valor de Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Establece un valor de MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Establece un valor de MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Establece un valor de Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Establece un valor de NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Establece un valor de NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Establece un valor que indica si IsNull está establecido o no. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Establece un valor que indica si Overallocated está establecido o no. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Establece un valor de OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Establece un valor de OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Establece un valor de OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Establece un valor de PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Establece un valor de PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Establece un valor de Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Establece un valor de RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Establece un valor de RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Establece un valor de RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Establece un valor de RemainingWork. |
| [setSV(double value)](#setSV-double-) | Establece un valor de SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Establece un valor de StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Establece un valor de StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Establece un valor de Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Establece un valor que indica si IsTeamAssignmentPool está establecido o no. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Establece una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto. |
| [setType(int value)](#setType-int-) | Establece un valor de Type. |
| [setUid(int value)](#setUid-int-) | Establece un valor de Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Establece un valor de WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Establece un valor de Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Establece un valor de WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Establece un valor de Workgroup. |
| [toString()](#toString--) | Devuelve la representación corta en forma de cadena de la instancia de la clase [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Devuelve el valor al que la propiedad está mapeada en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clave de propiedad especificada. [Rsc](../../com.aspose.tasks/rsc) para obtener la clave de propiedad. |

**Returns:**
T - el valor al que la propiedad está asignada en este contenedor.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Mapea la propiedad especificada al valor especificado en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clave de propiedad especificada. [Rsc](../../com.aspose.tasks/rsc) para obtener la clave de propiedad. |
| val | T | el valor. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Obtiene un valor que indica si CanLevel está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Elimina un recurso y sus asignaciones del proyecto.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | La instancia especificada de la clase [Resource](../../com.aspose.tasks/resource) para comparar con esta instancia. |

**Returns:**
boolean - **True** si la instancia especificada de la clase [Resource](../../com.aspose.tasks/resource) tiene el mismo valor de Uid que esta instancia; de lo contrario, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto para comparar con esta instancia. |

**Returns:**
boolean - **True** si el objeto especificado es un Resource que tiene el mismo valor de Uid que esta instancia; de lo contrario, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Obtiene un valor de ACWP.

**Returns:**
double - un valor de ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Obtiene un valor de AccrueAt.

**Returns:**
int - un valor de AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Obtiene un valor de ActiveDirectoryGuid.

**Returns:**
java.lang.String - un valor de ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Obtiene un valor de ActualCost.

**Returns:**
java.math.BigDecimal - un valor de ActualCost.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Obtiene un valor de ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - un valor de ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Obtiene un valor de ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Obtiene un valor de ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Obtiene un valor de ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Obtiene un valor de ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Obtiene un valor de AssignmentOwner.

**Returns:**
java.lang.String - un valor de AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Obtiene un valor de AssignmentOwnerGuid.

**Returns:**
java.lang.String - un valor de AssignmentOwnerGuid.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Obtiene una colección de asignaciones de recursos para este objeto.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Obtiene la instancia de la clase [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). La colección de períodos durante los cuales un recurso está disponible.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Obtiene un valor de AvailableFrom.

**Returns:**
java.util.Date - un valor de AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Obtiene un valor de AvailableTo.

**Returns:**
java.util.Date - un valor de AvailableTo.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Obtiene un valor de BCWP.

**Returns:**
double - un valor de BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Obtiene un valor de BCWS.

**Returns:**
double - un valor de BCWS.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Obtiene una instancia de BaselineCollection para este objeto. Los valores de referencia para un recurso.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Obtiene un valor de BookingType.

**Returns:**
int - un valor de BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Obtiene un valor de BudgetCost.

**Returns:**
java.math.BigDecimal - un valor de BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Obtiene un valor de BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Obtiene un valor de CV.

**Returns:**
double - un valor de CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Obtiene un valor de Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Obtiene un valor de Code.

**Returns:**
java.lang.String - un valor de Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtiene un valor de Cost.

**Returns:**
java.math.BigDecimal - un valor de Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Obtiene un valor de CostCenter.

**Returns:**
java.lang.String - un valor de CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Obtiene un valor de CostPerUse.

**Returns:**
java.math.BigDecimal - un valor de CostPerUse.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Obtiene un valor de CostVariance.

**Returns:**
double - un valor de CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Obtiene un valor de Created.

**Returns:**
java.util.Date - un valor de Created.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Obtiene un valor de EMailAddress.

**Returns:**
java.lang.String - un valor de EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Obtiene los valores de un atributo extendido.

--------------------

Se requieren dos piezas de datos - un puntero de regreso a la tabla de atributos extendidos que se especifica ya sea por el ID único o el ID de Campo, y el valor que se especifica ya sea con el valor, o un puntero de regreso a la lista de valores.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtiene un valor de Finish.

**Returns:**
java.util.Date - un valor de Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Obtiene un valor de Group.

**Returns:**
java.lang.String - un valor de Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Obtiene un valor de Guid.

**Returns:**
java.lang.String - un valor de Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Obtiene el título o texto explicativo de un hipervínculo asociado a un recurso.

**Returns:**
java.lang.String - el título o texto explicativo de un hipervínculo asociado a un recurso.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Obtiene la dirección de un hipervínculo asociado a un recurso.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

**Returns:**
java.lang.String - la dirección de un hipervínculo asociado a un recurso.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Obtiene la ubicación específica en un documento de un hipervínculo asociado a un recurso.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

**Returns:**
java.lang.String - la ubicación específica en un documento en un hipervínculo asociado a un recurso.
### getId() {#getId--}
```
public final int getId()
```


Obtiene un valor de Id.

**Returns:**
int - un valor de Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Obtiene un valor que indica si Inactive está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Obtiene un valor de Initials.

**Returns:**
java.lang.String - un valor de Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Obtiene recursos hijos.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - recursos secundarios.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Obtiene un valor de MaterialLabel.

**Returns:**
java.lang.String - un valor de MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Obtiene un valor de MaxUnits.

**Returns:**
double - un valor de MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Obtiene un valor de Name.

**Returns:**
java.lang.String - un valor de Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Obtiene un valor de NotesRTF.

**Returns:**
java.lang.String - un valor de NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Obtiene un valor de NotesText.

**Returns:**
java.lang.String - un valor de NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Obtiene un objeto OutlineCodeCollection. El valor de un código de esquema.

--------------------

Se requieren dos piezas de datos: un puntero a la tabla de códigos de esquema que se especifica mediante FieldID, y el valor que se especifica ya sea mediante el puntero ValueID o ValueGUID a la lista de valores.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Obtiene un valor que indica si Overallocated está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Obtiene un valor de OvertimeCost.

**Returns:**
java.math.BigDecimal - un valor de OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Obtiene un valor de OvertimeRate.

**Returns:**
java.math.BigDecimal - un valor de OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Obtiene un valor de OvertimeRateFormat.

**Returns:**
int - un valor de OvertimeRateFormat.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Obtiene un valor de OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el proyecto principal para este contenedor.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Obtiene un valor de PeakUnits.

**Returns:**
double - un valor de PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Obtiene un valor de PercentWorkComplete.

**Returns:**
int - un valor de PercentWorkComplete.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Obtiene un valor de Phonetics.

**Returns:**
java.lang.String - un valor de Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Obtiene la instancia de la clase [RateCollection](../../com.aspose.tasks/ratecollection) para este objeto. La colección de períodos y tarifas asociadas a cada una.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Obtiene un valor de RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Obtiene un valor de RemainingCost.

**Returns:**
java.math.BigDecimal - un valor de RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Obtiene un valor de RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - un valor de RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Obtiene un valor de RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Obtiene un valor de RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


Obtiene un valor de SV.

**Returns:**
double - un valor de SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Obtiene un valor de StandardRate.

**Returns:**
java.math.BigDecimal - un valor de StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Obtiene un valor de StandardRateFormat.

**Returns:**
int - un valor de StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtiene un valor de Start.

**Returns:**
java.util.Date - un valor de Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtiene una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto.

--------------------

Lectura compatible solo con formato XML.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Devuelve [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto con los valores de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dentro de las fechas de inicio y fin proporcionadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | La fecha de inicio para los datos con fase de tiempo. |
| fin | java.util.Date | La fecha de finalización de los datos con fase de tiempo. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Devuelve una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto con los valores de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dentro de las fechas de inicio y fin proporcionadas del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | La fecha de inicio de los datos con fase de tiempo. |
| fin | java.util.Date | La fecha de finalización de los datos con fase de tiempo. |
| timephasedType | byte | El tipo de datos con fase de tiempo ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Obtiene un valor de Type.

**Returns:**
int - un valor de Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtiene un valor de Uid.

**Returns:**
int - un valor de Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Obtiene un valor de WindowsUserAccount.

**Returns:**
java.lang.String - un valor de WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtiene un valor de Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Obtiene un valor de WorkVariance.

**Returns:**
double - un valor de WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Obtiene un valor de Workgroup.

**Returns:**
int - un valor de Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Reservado para uso interno.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Obtiene un valor que indica si IsBudget está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Obtiene un valor que indica si IsCostResource está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Obtiene un valor que indica si IsEnterprise está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Obtiene un valor que indica si IsGeneric está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Obtiene un valor que indica si IsNull está establecido o no.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Obtiene la bandera que indica si el recurso es un recurso raíz. El recurso raíz es un recurso especial que está destinado a soportar los internos de los formatos de MS Project y no está destinado a ser utilizado directamente desde el código del usuario.

**Returns:**
boolean - la bandera que indica si el recurso es un recurso raíz.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Obtiene un valor que indica si IsTeamAssignmentPool está establecido o no.

**Returns:**
boolean - un valor que indica si IsTeamAssignmentPool está configurado o no.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Mapea la propiedad especificada al valor especificado en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | la clave de propiedad especificada. [Rsc](../../com.aspose.tasks/rsc) para obtener la clave de propiedad. |
| val | java.util.Date | el valor. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Establece un valor de ACWP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Establece un valor de AccrueAt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Establece un valor de ActiveDirectoryGuid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Establece un valor de ActualCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de ActualCost. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Establece un valor de ActualOvertimeCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Establece un valor de ActualOvertimeWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Establece un valor de ActualOvertimeWorkProtected.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de ActualOvertimeWorkProtected. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Establece un valor de ActualWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Establece un valor de ActualWorkProtected.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Establece un valor de AssignmentOwner.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Establece un valor de AssignmentOwnerGuid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de AssignmentOwnerGuid. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Establece un valor de AvailableFrom.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Establece un valor de AvailableTo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de AvailableTo. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Establece un valor de BCWP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Establece un valor de BCWS.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Establece un valor de BookingType.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de BookingType. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Establece un valor que indica si IsBudget está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si IsBudget está configurado o no. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Establece un valor de BudgetCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Establece un valor de BudgetWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Establece un valor de CV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Establece un valor de Calendar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | un valor de Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Establece un valor que indica si CanLevel está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si CanLevel está configurado o no. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Establece un valor de Code.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Establece un valor de Cost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Establece un valor de CostCenter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Establece un valor de CostPerUse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Establece un valor que indica si IsCostResource está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si IsCostResource está configurado o no. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Establece un valor de CostVariance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Establece un valor de Created.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Created. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Establece un valor de EMailAddress.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Establece un valor que indica si IsEnterprise está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si IsEnterprise está configurado o no. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Establece un valor de Finish.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Establece un valor que indica si IsGeneric está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si IsGeneric está configurado o no. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Establece un valor de Group.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Establece un valor de Guid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Establece el título o texto explicativo de un hipervínculo asociado a un recurso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el título o texto explicativo de un hipervínculo asociado a un recurso. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Establece la dirección de un hipervínculo asociado a un recurso.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la dirección de un hipervínculo asociado a un recurso. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Establece la ubicación específica en un documento en un hipervínculo asociado a un recurso.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la ubicación específica en un documento en un hipervínculo asociado a un recurso. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Establece un valor de Id.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Establece un valor que indica si Inactive está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si Inactive está configurado o no. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Establece un valor de Initials.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Establece un valor de MaterialLabel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Establece un valor de MaxUnits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Establece un valor de Name.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Establece un valor de NotesRTF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Establece un valor de NotesText.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Establece un valor que indica si IsNull está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si IsNull está configurado o no. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Establece un valor que indica si Overallocated está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valor que indica si Overallocated está configurado o no. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Establece un valor de OvertimeCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Establece un valor de OvertimeRate.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Establece un valor de OvertimeRateFormat.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de OvertimeRateFormat. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Establece un valor de OvertimeWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Establece un valor de PeakUnits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Establece un valor de PercentWorkComplete.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de PercentWorkComplete. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Establece un valor de Phonetics.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Phonetics. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Establece un valor de RegularWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Establece un valor de RemainingCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Establece un valor de RemainingOvertimeCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Establece un valor de RemainingOvertimeWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Establece un valor de RemainingWork.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de RemainingWork. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Establece un valor de SV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Establece un valor de StandardRate.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Establece un valor de StandardRateFormat.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Establece un valor de Start.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Establece un valor que indica si IsTeamAssignmentPool está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si IsTeamAssignmentPool está configurado o no. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Establece una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto.

--------------------

Lectura compatible solo con formato XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | una instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) para este objeto. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Establece un valor de Type.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Establece un valor de Uid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Establece un valor de WindowsUserAccount.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Establece un valor de Work.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Establece un valor de WorkVariance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Establece un valor de Workgroup.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena corta de la instancia de la clase [Resource](../../com.aspose.tasks/resource). Los detalles exactos de la representación no están especificados y pueden cambiar.

**Returns:**
java.lang.String - cadena corta que representa el objeto de recurso.
