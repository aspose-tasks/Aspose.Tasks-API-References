---
title: "ResourceAssignment"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una asignación de recurso en un proyecto."
type: docs
weight: 249
url: /es/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Representa una asignación de recurso en un proyecto.
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Devuelve el valor al que la propiedad está mapeada en este contenedor. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mapea la propiedad especificada al valor especificado en este contenedor. |
| [delete()](#delete--) | Elimina la asignación de recursos de la colección de asignaciones del proyecto. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getACWP()](#getACWP--) | Obtiene un valor de ACWP. |
| [getActualCost()](#getActualCost--) | Obtiene un valor de ActualCost. |
| [getActualFinish()](#getActualFinish--) | Obtiene un valor de ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Obtiene un valor de ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Obtiene un valor de ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Obtiene un valor de ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Obtiene un valor de ActualStart. |
| [getActualWork()](#getActualWork--) | Obtiene un valor de ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Obtiene un valor de ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Obtiene un valor de AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Obtiene un valor de AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Obtiene un valor de BCWP. |
| [getBCWS()](#getBCWS--) | Obtiene un valor de BCWS. |
| [getBaselines()](#getBaselines--) | Obtiene el objeto AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | Obtiene un valor de BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Obtiene un valor de BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Obtiene un valor de BudgetWork. |
| [getCV()](#getCV--) | Obtiene un valor de CV. |
| [getConfirmed()](#getConfirmed--) | Obtiene un valor que indica si Confirmed está establecido o no. |
| [getCost()](#getCost--) | Obtiene un valor de Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Obtiene un valor de CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Obtiene un valor de CostVariance. |
| [getCreated()](#getCreated--) | Obtiene un valor de Created. |
| [getDelay()](#getDelay--) | Obtiene un valor de Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtiene una instancia de la clase ExtendedAttributeCollection para este objeto. |
| [getFinish()](#getFinish--) | Obtiene un valor de Finish. |
| [getFinishVariance()](#getFinishVariance--) | Obtiene un valor de FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Obtiene un valor que indica si FixedMaterial está configurado o no. |
| [getGuid()](#getGuid--) | Obtiene el identificador único para esta asignación. |
| [getHyperlink()](#getHyperlink--) | Obtiene un valor de Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Obtiene un valor de HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Obtiene un valor de HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Obtiene un valor de LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Obtiene un valor que indica si LinkedFields está configurado o no. |
| [getMilestone()](#getMilestone--) | Obtiene un valor que indica si Milestone está configurado o no. |
| [getNotesRTF()](#getNotesRTF--) | Obtiene las notas de texto en formato RTF. |
| [getNotesText()](#getNotesText--) | Obtiene el texto plano de las notas extraído de los datos RTF. |
| [getOverallocated()](#getOverallocated--) | Obtiene un valor que indica si Overallocated está establecido o no. |
| [getOvertimeCost()](#getOvertimeCost--) | Obtiene un valor de OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Obtiene un valor de OvertimeWork. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto principal para esta asignación. |
| [getPeakUnits()](#getPeakUnits--) | Obtiene un valor de PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Obtiene un valor de PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Obtiene un valor de RateScale. |
| [getRegularWork()](#getRegularWork--) | Obtiene un valor de RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Obtiene un valor de RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Obtiene un valor de RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Obtiene un valor de RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Obtiene un valor de RemainingWork. |
| [getResource()](#getResource--) | El recurso asignado a una tarea. |
| [getResponsePending()](#getResponsePending--) | Obtiene un valor que indica si ResponsePending está configurado o no. |
| [getResume()](#getResume--) | Obtiene un valor de Resume. |
| [getSV()](#getSV--) | Obtiene un valor de SV. |
| [getStart()](#getStart--) | Obtiene un valor de Start. |
| [getStartVariance()](#getStartVariance--) | Obtiene un valor de StartVariance. |
| [getStop()](#getStop--) | Obtiene un valor de Stop. |
| [getSummary()](#getSummary--) | Obtiene un valor que indica si Summary está configurado o no. |
| [getTask()](#getTask--) | La tarea a la que se asigna un recurso. |
| [getTimephasedData()](#getTimephasedData--) | Obtiene la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene elementos de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) clase. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Devuelve el objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) con las instancias de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) clase dentro de las fechas de inicio y fin dadas de [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Devuelve la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene instancias de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) clase dentro de las fechas de inicio y fin dadas del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Obtiene la cantidad de trabajo faseado en el intervalo de fecha y hora especificado. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Obtiene la cantidad de trabajo faseado en el intervalo de fecha y hora especificado. |
| [getUid()](#getUid--) | Obtiene un valor de Uid. |
| [getUnits()](#getUnits--) | Obtiene un valor de Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Obtiene un valor que indica si UpdateNeeded está configurado o no. |
| [getVAC()](#getVAC--) | Obtiene un valor de VAC. |
| [getWork()](#getWork--) | Obtiene un valor de Work. |
| [getWorkContour()](#getWorkContour--) | Obtiene un valor de WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Obtiene un valor de WorkVariance. |
| [hasChildren()](#hasChildren--) | Obtiene un valor que indica que esta asignación de recursos tiene hijos. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Obtiene un valor que indica si HasFixedRateUnits está establecido o no. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Genera una lista de datos por fases de tiempo. |
| [setACWP(double value)](#setACWP-double-) | Establece un valor de ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Establece un valor de ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Establece un valor de ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Establece un valor de ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Establece un valor de ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Establece un valor de ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Establece un valor de ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Establece un valor de ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Establece un valor de AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Establece un valor de AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Establece un valor de BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Establece un valor de BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Establece un valor de BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Establece un valor de BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Establece un valor de BudgetWork. |
| [setCV(double value)](#setCV-double-) | Establece un valor de CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Establece un valor que indica si Confirmed está establecido o no. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Establece un valor de Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Establece un valor de CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Establece un valor de CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Establece un valor de Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Establece un valor de Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Establece una instancia de la clase ExtendedAttributeCollection para este objeto. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Establece un valor de Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Establece un valor de FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Establece un valor que indica si FixedMaterial está establecido o no. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Establece un valor que indica si HasFixedRateUnits está establecido o no. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Establece un identificador único para esta asignación. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Establece un valor de Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Establece un valor de HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Establece un valor de HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Establece un valor de LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Establece un valor que indica si LinkedFields está establecido o no. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Establece unidades para la asignación de un recurso material con consumo variable de material. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Establece un valor que indica si Milestone está establecido o no. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Establece las notas de texto en formato RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Establece el texto plano de las notas extraído de los datos RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Establece un valor que indica si Overallocated está establecido o no. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Establece un valor de OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Establece un valor de PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Establece un valor de PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Establece un valor de RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Establece un valor de RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Establece un valor de RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Establece un valor de RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Establece un valor de RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Establece un valor de RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | El recurso asignado a una tarea. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Establece un valor que indica si ResponsePending está establecido o no. |
| [setResume(Date value)](#setResume-java.util.Date-) | Establece un valor de Resume. |
| [setSV(double value)](#setSV-double-) | Establece un valor de SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Establece un valor de Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Establece un valor de StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Establece un valor de Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Establece un valor que indica si Summary está establecido o no. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | La tarea a la que se asigna un recurso. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Establece la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene elementos de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)). |
| [setUid(int value)](#setUid-int-) | Establece un valor de Uid. |
| [setUnits(double value)](#setUnits-double-) | Establece un valor de Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Establece un valor que indica si UpdateNeeded está establecido o no. |
| [setVAC(double value)](#setVAC-double-) | Establece un valor de VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Establece un valor de Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Establece un valor de WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Establece un valor de WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Divide la tarea en dos partes. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Genera una lista de datos por fases de tiempo basada en la duración de la tarea y la fecha de inicio programada. |
| [toString()](#toString--) | Devuelve una representación corta en forma de cadena de la instancia de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Devuelve el valor al que la propiedad está mapeada en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clave de propiedad especificada. [Asn](../../com.aspose.tasks/asn) para obtener la clave de propiedad. |

**Returns:**
T - el valor al que la propiedad está asignada en este contenedor.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mapea la propiedad especificada al valor especificado en este contenedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clave de propiedad especificada. [Asn](../../com.aspose.tasks/asn) para obtener la clave de propiedad. |
| val | T | el valor. |

### delete() {#delete--}
```
public final void delete()
```


Elimina la asignación de recursos de la colección de asignaciones del proyecto.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | La instancia especificada de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment) para comparar con esta instancia. |

**Returns:**
boolean - **True** si la instancia especificada de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment) tiene el mismo valor UID que esta instancia; de lo contrario, **false**.
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
boolean - **True** si o es un ResourceAssignment que asigna el mismo recurso y tarea que esta instancia; de lo contrario, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Obtiene un valor de ACWP.

**Returns:**
double - un valor de ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Obtiene un valor de ActualCost.

**Returns:**
java.math.BigDecimal - un valor de ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Obtiene un valor de ActualFinish.

**Returns:**
java.util.Date - un valor de ActualFinish.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Obtiene un valor de ActualStart.

**Returns:**
java.util.Date - un valor de ActualStart.
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
public final AssignmentBaselineCollection getBaselines()
```


Obtiene el objeto AssignmentBaselineCollection. La colección de valores de línea base asociados a una asignación.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Obtiene un valor que indica si Confirmed está establecido o no.

**Returns:**
boolean - un valor que indica si Confirmed está establecido o no.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtiene un valor de Cost.

**Returns:**
java.math.BigDecimal - un valor de Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Obtiene un valor de CostRateTableType.

**Returns:**
int - un valor de CostRateTableType.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Obtiene un valor de Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Obtiene una instancia de la clase ExtendedAttributeCollection para este objeto.

--------------------

Lectura compatible solo con formato XML.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtiene un valor de Finish.

**Returns:**
java.util.Date - un valor de Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Obtiene un valor de FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Obtiene un valor que indica si FixedMaterial está configurado o no.

**Returns:**
boolean - un valor que indica si FixedMaterial está establecido o no.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtiene el identificador único para esta asignación.

**Returns:**
java.util.UUID - identificador único para esta asignación.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Obtiene un valor de Hyperlink.

**Returns:**
java.lang.String - un valor de Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Obtiene un valor de HyperlinkAddress.

**Returns:**
java.lang.String - un valor de HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Obtiene un valor de HyperlinkSubAddress.

**Returns:**
java.lang.String - un valor de HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Reservado para uso interno.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Obtiene un valor de LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Obtiene un valor que indica si LinkedFields está configurado o no.

**Returns:**
boolean - un valor que indica si LinkedFields está configurado o no.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Obtiene un valor que indica si Milestone está configurado o no.

**Returns:**
boolean - un valor que indica si Milestone está configurado o no.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Obtiene las notas de texto en formato RTF.

--------------------

Compatible solo con formatos MPP.

**Returns:**
java.lang.String - las notas de texto en formato RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Obtiene el texto plano de las notas extraído de los datos RTF.

**Returns:**
java.lang.String - texto plano de las notas extraído de los datos RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Obtiene un valor que indica si Overallocated está establecido o no.

**Returns:**
boolean - un valor que indica si Overallocated está configurado o no.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Obtiene un valor de OvertimeCost.

**Returns:**
java.math.BigDecimal - un valor de OvertimeCost.
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


Obtiene el proyecto principal para esta asignación.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Obtiene un valor de RateScale.

**Returns:**
int - un valor de RateScale.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


El recurso asignado a una tarea.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Obtiene un valor que indica si ResponsePending está configurado o no.

**Returns:**
boolean - un valor que indica si ResponsePending está configurado o no.
### getResume() {#getResume--}
```
public final Date getResume()
```


Obtiene un valor de Resume.

**Returns:**
java.util.Date - un valor de Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Obtiene un valor de SV.

**Returns:**
double - un valor de SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtiene un valor de Start.

**Returns:**
java.util.Date - un valor de Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Obtiene un valor de StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Obtiene un valor de Stop.

**Returns:**
java.util.Date - un valor de Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Obtiene un valor que indica si Summary está configurado o no.

**Returns:**
boolean - un valor que indica si Summary está configurado o no.
### getTask() {#getTask--}
```
public final Task getTask()
```


La tarea a la que se asigna un recurso.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtiene la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene elementos de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) clase.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Devuelve el objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) con las instancias de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) clase dentro de las fechas de inicio y fin dadas de [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | La fecha de inicio de los datos con fase de tiempo. |
| fin | java.util.Date | La fecha de finalización de los datos con fase de tiempo. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Devuelve la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene instancias de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) clase dentro de las fechas de inicio y fin dadas del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | La fecha de inicio de los datos con fase de tiempo. |
| fin | java.util.Date | La fecha de finalización de los datos con fase de tiempo. |
| timephasedType | byte | El tipo de datos con fase de tiempo ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Obtiene la cantidad de trabajo faseado en el intervalo de fecha y hora especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Inicio del intervalo de fecha y hora. |
| fin | java.util.Date | Fin del intervalo de fecha y hora. |

**Returns:**
double - cantidad de trabajo por fases de tiempo para el intervalo de fecha y hora especificado.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Obtiene la cantidad de trabajo faseado en el intervalo de fecha y hora especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Inicio del intervalo de fecha y hora. |
| fin | java.util.Date | Fin del intervalo de fecha y hora. |
| timephasedDataType | byte | Tipo de los datos por fases de tiempo a usar. |

**Returns:**
double - cantidad de trabajo por fases de tiempo para el intervalo de fecha y hora especificado.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtiene un valor de Uid.

**Returns:**
int - un valor de Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Obtiene un valor de Units.

**Returns:**
double - un valor de Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Obtiene un valor que indica si UpdateNeeded está configurado o no.

**Returns:**
boolean - un valor que indica si UpdateNeeded está configurado o no.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Obtiene un valor de VAC.

**Returns:**
double - un valor de VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtiene un valor de Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Obtiene un valor de WorkContour.

**Returns:**
int - un valor de WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Obtiene un valor de WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Obtiene un valor que indica que esta asignación de recursos tiene hijos.

**Returns:**
boolean - Siempre falso.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Obtiene un valor que indica si HasFixedRateUnits está establecido o no.

**Returns:**
boolean - un valor que indica si HasFixedRateUnits está configurado o no.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Genera una lista de datos por fases de tiempo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | La fecha de inicio especificada. |
| time | double | El tiempo de trabajo especificado. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | El calendario de trabajo especificado. |
| lista | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | La lista de datos con fase de tiempo. |
| isWorking | boolean | La bandera especificada que indica si los datos con fase de tiempo están activos o no. |
| type | int | El tipo de datos con fase de tiempo especificado. |

**Returns:**
java.util.Date - Una fecha máxima de la lista o fecha de inicio si la lista está vacía.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Establece un valor de ACWP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Establece un valor de ActualCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Establece un valor de ActualFinish.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de ActualFinish. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Establece un valor de ActualStart.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de ActualStart. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Establece un valor que indica si Confirmed está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Confirmed está establecido o no. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Establece un valor de Cost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Establece un valor de CostRateTableType.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de CostRateTableType. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Establece un valor de Delay.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Establece una instancia de la clase ExtendedAttributeCollection para este objeto.

--------------------

Lectura compatible solo con formato XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | una instancia de la clase ExtendedAttributeCollection para este objeto. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Establece un valor de Finish.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Establece un valor de FinishVariance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Establece un valor que indica si FixedMaterial está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si FixedMaterial está establecido o no. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Establece un valor que indica si HasFixedRateUnits está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si HasFixedRateUnits está establecido o no. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Establece un identificador único para esta asignación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID | identificador único para esta asignación. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Establece un valor de Hyperlink.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Establece un valor de HyperlinkAddress.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Establece un valor de HyperlinkSubAddress.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor de HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Establece un valor de LevelingDelay.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Establece un valor que indica si LinkedFields está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si LinkedFields está establecido o no. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Establece unidades para la asignación de un recurso material con consumo de material variable. El consumo de material variable significa que a medida que la duración de la asignación cambia, la cantidad de materiales utilizados cambia proporcionalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| unidades | double | Número de unidades acumuladas en el período de tiempo. |
|  | rateScaleType | int | Período de tiempo en el que se acumula el valor de la unidad. |

--------------------

Por ejemplo, para establecer '123/mes', SetUnitsScaled(123D, RateScaleType.Month) debe llamarse. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Establece un valor que indica si Milestone está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Milestone está establecido o no. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Establece las notas de texto en formato RTF.

--------------------

Compatible solo con formatos MPP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | las notas de texto en formato RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Establece el texto plano de las notas extraído de los datos RTF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | texto sin formato de las notas extraído de los datos RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Establece un valor que indica si Overallocated está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Overallocated está configurado o no. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Establece un valor de OvertimeCost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor de OvertimeCost. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Establece un valor de RateScale.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de RateScale. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


El recurso asignado a una tarea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | el recurso asignado a una tarea. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Establece un valor que indica si ResponsePending está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si ResponsePending está establecido o no. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Establece un valor de Resume.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Establece un valor de SV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Establece un valor de Start.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Establece un valor de StartVariance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Establece un valor de Stop.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor de Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Establece un valor que indica si Summary está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Summary está establecido o no. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


La tarea a la que se asigna un recurso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tarea a la que se asigna un recurso. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Establece la instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) que contiene elementos de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | la instancia de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) clase que contiene elementos de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) clase. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Establece un valor de Uid.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Establece un valor de Units.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Establece un valor que indica si UpdateNeeded está establecido o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si UpdateNeeded está establecido o no. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Establece un valor de VAC.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un valor de VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Establece un valor de Work.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Establece un valor de WorkContour.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor de WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Establece un valor de WorkVariance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valor de WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Divide la tarea en dos partes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | El comienzo de la interrupción del trabajo sobre la cual dividir. |
| finalizar | java.util.Date | El final de la interrupción del trabajo sobre la cual dividir. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | El calendario sobre el cual dividir. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Genera una lista de datos por fases de tiempo basada en la duración de la tarea y la fecha de inicio programada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | El calendario del cual generar datos por fases temporales. |

### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena corta de la instancia de la clase [ResourceAssignment](../../com.aspose.tasks/resourceassignment). Los detalles exactos de la representación no están especificados y pueden cambiar.

**Returns:**
java.lang.String - cadena corta que representa el objeto de asignación.
