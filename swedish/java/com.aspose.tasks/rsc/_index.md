---
title: "Rsc"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar stödda egenskaper för Resource-objektet."
type: docs
weight: 271
url: /sv/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

Representerar de stödjade egenskaperna för `Resource`-objektet.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | Bestämmer hur och när resursens standard- och övertidskostnader ska debiteras eller bokföras på kostnaden för en uppgift. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | Den Active Directory Guid för en resurs. |
| [ACTUAL_COST](#ACTUAL-COST) | Kostnader som uppkommit för arbete som redan utförts av resurser på deras uppgifter, tillsammans med eventuella andra registrerade kostnader som är kopplade till uppgiften. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Kostnader som uppkommit för övertidsarbete som redan utförts på uppgifter av tilldelade resurser. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | Den faktiska mängden övertidsarbete som redan utförts av resurs som är tilldelad uppgifter. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | Mängden arbete genom vilket faktiskt övertidsarbete skyddas. |
| [ACTUAL_WORK](#ACTUAL-WORK) | Mängden arbete som redan har utförts av resurs som är tilldelad uppgifter. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | Mängden arbete genom vilket faktiskt arbete skyddas. |
| [ACWP](#ACWP) | Den faktiska kostnaden för ett arbete som utförts av en resurs för projektet hittills. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | Namnet på en tilldelningsägare. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | GUID för en tilldelningsägare. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | Startdatumet då en resurs är tillgänglig för arbete med de enheter som specificerats för den aktuella tidsperioden. |
| [AVAILABLE_TO](#AVAILABLE-TO) | Slutdatumet då en resurs är tillgänglig för arbete med de enheter som specificerats för den aktuella tidsperioden. |
| [BCWP](#BCWP) | Den budgeterade kostnaden för ett arbete som utförts av en resurs för projektet hittills. |
| [BCWS](#BCWS) | Budgetkostnaden för ett arbete som är schemalagt för en resurs. |
| [BOOKING_TYPE](#BOOKING-TYPE) | Bokningstypen för en resurs. |
| [BUDGET_COST](#BUDGET-COST) | Budgetkostnader för budgetkostnadsresurser. |
| [BUDGET_WORK](#BUDGET-WORK) | budgetarbete för budgetarbete och materialresurser. |
| [CALENDAR](#CALENDAR) | Kalendern för en resurs. |
| [CAN_LEVEL](#CAN-LEVEL) | Bestämmer om resursutjämning kan utföras på en resurs. |
| [CODE](#CODE) | Koden eller annan information om en resurs. |
| [COST](#COST) | Den totala planerade eller beräknade kostnaden för en resurs, baserad på kostnader som redan uppkommit för arbete utfört av resurser som tilldelats uppgifterna, samt kostnaderna som är planerade för återstående arbete. |
| [COST_CENTER](#COST-CENTER) | Anger vilket kostnadsställe de kostnader som ackumulerats av resursen ska debiteras till. |
| [COST_PER_USE](#COST-PER-USE) | Kostnaden som uppstår varje gång en resurs används. |
| [COST_VARIANCE](#COST-VARIANCE) | Skillnaden mellan grundkostnaden och den totala kostnaden för en resurs. |
| [CREATED](#CREATED) | Datum och tid då en resurs lades till i projektet. |
| [CV](#CV) | Den intjänade värde‑kostnadsvariansen fram till det aktuella projektstatusdatumet. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | Resursens e‑postadress. |
| [FINISH](#FINISH) | Datumet då en resurs är schemalagd att slutföra arbete på alla tilldelade uppgifter. |
| [GROUP](#GROUP) | Den grupp som en resurs tillhör. |
| [GUID](#GUID) | Innehåller den genererade unika identifieringskoden för resursen. |
| [HYPERLINK](#HYPERLINK) | Titeln eller förklarande text för en hyperlänk som är associerad med en resurs. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | Adressen för en hyperlänk som är associerad med en resurs. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | Den specifika platsen i ett dokument i en hyperlänk som är associerad med en uppgift. |
| [ID](#ID) | Positionsidentifieraren för en resurs i resurslistan. |
| [INACTIVE](#INACTIVE) | Avgör om en resurs har gjorts inaktiv av en användare med administrativa rättigheter. |
| [INITIALS](#INITIALS) | Resursens initialer. |
| [IS_BUDGET](#IS-BUDGET) | Avgör om en arbets-, material- eller kostnadsresurs är en budgetresurs. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | Avgör om en resurs är en kostnadsresurs. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | Visar om en resurs kommer från företagets resurspool (true) eller den lokala resurspoolen (false). |
| [IS_GENERIC](#IS-GENERIC) | Avgör om en resurs är generisk eller inte. |
| [IS_NULL](#IS-NULL) | Avgör om en resurs är null. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | Visar om den aktuella resursen är en teamresurs. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | Måttenheten för materialresursen. |
| [MAX_UNITS](#MAX-UNITS) | Det maximala antalet enheter som representerar den högsta kapaciteten som en resurs är tillgänglig för att utföra uppgifter under den aktuella tidsperioden. |
| [NAME](#NAME) | Namnet på en resurs. |
| [NOTES_RTF](#NOTES-RTF) | Textanteckningarna i RTF-format. |
| [NOTES_TEXT](#NOTES-TEXT) | Anteckningarnas rena text extraherad från RTF-data. |
| [OVERALLOCATED](#OVERALLOCATED) | Anger om en resurs är tilldelad mer arbete på en specifik uppgift eller alla uppgifter än vad som kan slutföras inom normal arbetskapacitet. |
| [OVERTIME_COST](#OVERTIME-COST) | Den totala övertidskostnaden för en resurs på alla tilldelade uppgifter. |
| [OVERTIME_RATE](#OVERTIME-RATE) | Timlönen för övertidsarbete utfört av en resurs. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | De enheter som Microsoft Project använder för att visa övertidsräntan. |
| [OVERTIME_WORK](#OVERTIME-WORK) | Mängden övertid som är schemalagd att utföras av en resurs på en uppgift och debiteras enligt övertidsräntorna för de inblandade resurserna. |
| [PEAK_UNITS](#PEAK-UNITS) | Den maximala tilldelningsenheten för en resurs vid varje given tidpunkt för alla uppgifter som resursen är tilldelad. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | Procentandelen av arbetet som är slutfört för alla uppgifter. |
| [PHONETICS](#PHONETICS) | Den fonetiska stavningen av resursnamnet. |
| [REGULAR_WORK](#REGULAR-WORK) | Den totala mängden icke-övertidsarbete som är schemalagd att utföras av resursen. |
| [REMAINING_COST](#REMAINING-COST) | Den återstående schemalagda kostnaden som kommer att uppstå vid slutförandet av det återstående schemalagda arbetet. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | Den återstående schemalagda övertidskostnaden för en resurs. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | Mängden återstående schemalagda övertid. |
| [REMAINING_WORK](#REMAINING-WORK) | Den tid som fortfarande krävs för att slutföra en uppgift eller en uppgiftsuppsättning. |
| [STANDARD_RATE](#STANDARD-RATE) | Timlönen för reguljärt, icke-övertidsarbete utfört av en resurs. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | De enheter som Microsoft Project använder för att visa standardräntan. |
| [START](#START) | Datumet då en tilldelad resurs är schemalagd att börja arbeta på en uppgift. |
| [SV](#SV) | Den intjänade värdeplanens avvikelse fram till projektets statusdatum. |
| [TYPE](#TYPE) | Typen av en resurs. |
| [UID](#UID) | Den unika identifieraren för en resurs. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | NT-kontot som är kopplat till en resurs. |
| [WORK](#WORK) | Den totala tidsmängden som är schemalagd för en resurs på en uppgift. |
| [WORKGROUP](#WORKGROUP) | Typen av en arbetsgrupp som en resurs tillhör. |
| [WORK_VARIANCE](#WORK-VARIANCE) | Skillnaden mellan baslinjearbetet för en resurs och det för närvarande schemalagda arbetet. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


Bestämmer hur och när resursens standard- och övertidskostnader ska debiteras eller bokföras på kostnaden för en uppgift.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


Den Active Directory Guid för en resurs.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Kostnader som uppkommit för arbete som redan utförts av resurser på deras uppgifter, tillsammans med eventuella andra registrerade kostnader som är kopplade till uppgiften.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Kostnader som uppkommit för övertidsarbete som redan utförts på uppgifter av tilldelade resurser.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


Den faktiska mängden övertidsarbete som redan utförts av resurs som är tilldelad uppgifter.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


Mängden arbete genom vilket faktiskt övertidsarbete skyddas.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


Mängden arbete som redan har utförts av resurs som är tilldelad uppgifter.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


Mängden arbete genom vilket faktiskt arbete skyddas.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


Den faktiska kostnaden för ett arbete som utförts av en resurs för projektet hittills.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


Namnet på en tilldelningsägare.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


GUID för en tilldelningsägare.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


Startdatumet då en resurs är tillgänglig för arbete med de enheter som specificerats för den aktuella tidsperioden.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


Slutdatumet då en resurs är tillgänglig för arbete med de enheter som specificerats för den aktuella tidsperioden.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


Den budgeterade kostnaden för ett arbete som utförts av en resurs för projektet hittills.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


Budgetkostnaden för ett arbete som är schemalagt för en resurs.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


Bokningstypen för en resurs.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Budgetkostnader för budgetkostnadsresurser. Budgetresurser tilldelas endast till projektets sammanfattningsuppgift.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


budgetarbete för budgetarbete och materialresurser. Budgetresurser tilldelas endast till projektets sammanfattningsuppgift.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


Kalendern för en resurs.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


Bestämmer om resursutjämning kan utföras på en resurs.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


Koden eller annan information om en resurs.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


Den totala planerade eller beräknade kostnaden för en resurs, baserad på kostnader som redan uppkommit för arbete utfört av resurser som tilldelats uppgifterna, samt kostnaderna som är planerade för återstående arbete.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


Anger vilket kostnadsställe de kostnader som ackumulerats av resursen ska debiteras till.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


Kostnaden som uppstår varje gång en resurs används.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


Skillnaden mellan grundkostnaden och den totala kostnaden för en resurs.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


Datum och tid då en resurs lades till i projektet.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


Den intjänade värde kostnadsvariansen fram till projektets statusdatum. CV är skillnaden mellan uppgiftens BCWP (budgeterad kostnad för utfört arbete) och ACWP (faktisk kostnad för utfört arbete).

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


Resursens e‑postadress.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


Datumet då en resurs är schemalagd att slutföra arbete på alla tilldelade uppgifter.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


Den grupp som en resurs tillhör.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


Innehåller den genererade unika identifieringskoden för resursen.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


Titeln eller förklarande text för en hyperlänk som är associerad med en resurs.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


Adressen för en hyperlänk som är associerad med en resurs.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


Den specifika platsen i ett dokument i en hyperlänk som är associerad med en uppgift.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


Positionsidentifieraren för en resurs i resurslistan.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


Avgör om en resurs har gjorts inaktiv av en användare med administrativa rättigheter.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


Resursens initialer.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


Avgör om en arbets-, material- eller kostnadsresurs är en budgetresurs.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


Avgör om en resurs är en kostnadsresurs.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


Visar om en resurs kommer från företagets resurspool (true) eller den lokala resurspoolen (false).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


Avgör om en resurs är generisk eller inte.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Avgör om en resurs är null.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


Visar om den aktuella resursen är en teamresurs.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


Måttenheten för materialresursen.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


Det maximala antalet enheter som representerar den högsta kapaciteten som en resurs är tillgänglig för att utföra uppgifter under den aktuella tidsperioden.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


Namnet på en resurs.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


Textanteckningarna i RTF-format.

--------------------

Stöds endast för MPP-format.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


Anteckningarnas rena text extraherad från RTF-data.

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


Anger om en resurs är tilldelad mer arbete på en specifik uppgift eller alla uppgifter än vad som kan slutföras inom normal arbetskapacitet.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


Den totala övertidskostnaden för en resurs på alla tilldelade uppgifter.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


Timlönen för övertidsarbete utfört av en resurs.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


De enheter som Microsoft Project använder för att visa övertidsräntan.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


Mängden övertid som är schemalagd att utföras av en resurs på en uppgift och debiteras enligt övertidsräntorna för de inblandade resurserna.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


Den maximala tilldelningsenheten för en resurs vid varje given tidpunkt för alla uppgifter som resursen är tilldelad.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


Procentandelen av arbetet som är slutfört för alla uppgifter.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


Den fonetiska stavningen av resursnamnet. Endast för användning med japanska.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


Den totala mängden icke-övertidsarbete som är schemalagd att utföras av resursen.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


Den återstående schemalagda kostnaden som kommer att uppstå vid slutförandet av det återstående schemalagda arbetet.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


Den återstående schemalagda övertidskostnaden för en resurs.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


Mängden återstående schemalagda övertid.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


Den tid som fortfarande krävs för att slutföra en uppgift eller en uppgiftsuppsättning.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


Timlönen för reguljärt, icke-övertidsarbete utfört av en resurs.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


De enheter som Microsoft Project använder för att visa standardräntan.

### START {#START}
```
public static final Key<Date,Byte> START
```


Datumet då en tilldelad resurs är schemalagd att börja arbeta på en uppgift.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


Den intjänade värde schemaläggningsvariansen fram till projektets statusdatum. SV är skillnaden mellan budgeterad kostnad för utfört arbete (BCWP) och budgeterad kostnad för schemalagt arbete (BCWS).

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


Typen av en resurs.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


Den unika identifieraren för en resurs.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


NT-kontot som är kopplat till en resurs.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


Den totala tidsmängden som är schemalagd för en resurs på en uppgift.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


Typen av en arbetsgrupp som en resurs tillhör.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


Skillnaden mellan baslinjearbetet för en resurs och det för närvarande schemalagda arbetet.

