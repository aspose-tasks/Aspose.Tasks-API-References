---
title: "Tsk"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar egenskaper för objektet."
type: docs
weight: 328
url: /sv/java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

Representerar egenskaper för [Task](../../com.aspose.tasks/task)-objektet.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | Representerar aktivitets‑id‑fältet – en uppgifts unika identifierare som används av Primavera. |
| [ACTUAL_COST](#ACTUAL-COST) | Kostnader som uppkommit för arbete som redan utförts av resurser på deras uppgifter, tillsammans med eventuella andra registrerade kostnader som är kopplade till uppgiften. |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | Tidsintervallet för faktiskt arbetstid för en uppgift, baserat på den schemalagda varaktigheten och aktuellt återstående arbete eller färdigställt procenttal. |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | Datumet då en uppgift slutfördes. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Kostnader som uppkommit för övertidsarbete som redan utförts på uppgifter av tilldelade resurser. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | Den faktiska mängden övertidsarbete som redan utförts av resurser som tilldelats uppgifter. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | Varaktigheten under vilken faktiskt övertidsarbete är skyddat. |
| [ACTUAL_START](#ACTUAL-START) | Datumet och tiden då en uppgift faktiskt påbörjades. |
| [ACTUAL_WORK](#ACTUAL-WORK) | Mängden arbete som redan har utförts av resurser som tilldelats uppgifter. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | Varaktigheten under vilken faktiskt arbete är skyddat. |
| [ACWP](#ACWP) | Kostnader som uppkommit för arbete som redan utförts på en uppgift, fram till projektets statusdatum eller dagens datum. |
| [BCWP](#BCWP) | Det kumulativa värdet av uppgiftens färdigställt procenttal multiplicerat med de tidsfasade grundkostnaderna. |
| [BCWS](#BCWS) | De kumulativa tidsfasade grundkostnaderna fram till statusdatumet eller dagens datum. |
| [BUDGET_COST](#BUDGET-COST) | Budgetkostnader för budgetkostnadsresurser. |
| [BUDGET_WORK](#BUDGET-WORK) | Budgetarbete för budgetarbete och materialresurser. |
| [CALENDAR](#CALENDAR) | Uppgiftens kalender. |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | Slutdatumet för en leverans. |
| [COMMITMENT_START](#COMMITMENT-START) | Startdatumet för en leverans. |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | Bestämmer om en uppgift har en associerad leverans eller ett beroende av en associerad leverans. |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | Det specifika datumet som är associerat med begränsningstypen. |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | Tillhandahåller val för vilken typ av begränsning som kan tillämpas vid schemaläggning av en uppgift. |
| [CONTACT](#CONTACT) | Namnet på den person som ansvarar för en uppgift. |
| [COST](#COST) | Den totala schemalagda eller beräknade kostnaden för en uppgift baserad på kostnader som redan uppkommit för arbete utfört av resurser som tilldelats uppgifterna, samt de kostnader som planeras för återstående arbete. |
| [COST_VARIANCE](#COST-VARIANCE) | Skillnaden mellan grundkostnaden och total kostnad för en uppgift, resurs eller tilldelning. |
| [CREATED](#CREATED) | Datumet då en uppgift skapades. |
| [CV](#CV) | Skillnaden mellan grundkostnaden och total kostnad för en uppgift. |
| [DEADLINE](#DEADLINE) | Ett måldatum som visar när en uppgift ska slutföras. |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | Bestämmer om uppgiften ska visas som en sammanfattningsuppgift. |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | Anger om en uppgift ska visas i en tidslinjevy. |
| [DURATION](#DURATION) | Den totala perioden av aktiv arbetstid för en uppgift som anges eller beräknas av Microsoft Project baserat på startdatum, slutdatum, kalendrar och andra schemaläggningsfaktorer. |
| [DURATION_TEXT](#DURATION-TEXT) | Returnerar uppgiftens varaktighetstext. |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | Skillnaden mellan grundlinjens varaktighet för en uppgift och den totala varaktigheten (aktuella uppskattningen) för en uppgift. |
| [EARLY_FINISH](#EARLY-FINISH) | Det tidigaste datumet då en uppgift eventuellt kan slutföras, baserat på tidiga slutdatum för föregående och efterföljande uppgifter, andra begränsningar och eventuell nivåfördröjning. |
| [EARLY_START](#EARLY-START) | Det tidigaste datumet då en uppgift eventuellt kan påbörjas, baserat på tidiga startdatum för föregående och efterföljande uppgifter och andra begränsningar. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | Bestämmer om fältet % färdig eller Fysiskt % färdig ska användas för att beräkna budgeterad kostnad för utfört arbete (BCWP). |
| [EXTERNAL_ID](#EXTERNAL-ID) | Om en uppgift är en extern uppgift innehåller den uppgiftens externa ID. |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | Källplatsen och uppgiftsidentifieraren för en extern uppgift. |
| [EXTERNAL_UID](#EXTERNAL-UID) | Innehåller den externa uppgiftens unika identifierare när uppgiften är extern. |
| [FINISH](#FINISH) | Det planerade slutdatumet för en uppgift. |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | Varaktigheten (i sekunder) mellan tidigt slut och sent slut datum. |
| [FINISH_TEXT](#FINISH-TEXT) | Returnerar uppgiftens slutttext. |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | Tiden som representerar skillnaden mellan grundlinjens slutdatum för en uppgift eller tilldelning och dess aktuella slutdatum. |
| [FIXED_COST](#FIXED-COST) | Visar eventuella kostnader för icke-resursuppgifter. |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | Bestämmer val för hur och när fasta kostnader ska debiteras eller bokföras till en uppgifts kostnad. |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | Tiden (i sekunder) som en uppgift kan fördröjas utan att fördröja några efterföljande uppgifter. |
| [GUID](#GUID) | De genererade unika identifieringskoderna för en uppgift. |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | Indikerar om uppgiften har en resurs tilldelad som har mer arbete på tilldelade uppgifter än vad som kan slutföras inom normal arbetskapacitet. |
| [HIDE_BAR](#HIDE-BAR) | Bestämmer om Gantt-stapeln för en uppgift är dold när den visas i Microsoft Project. |
| [HYPERLINK](#HYPERLINK) | Titeln eller förklarande text för en hyperlänk som är associerad med en uppgift. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | Adressen för en hyperlänk som är associerad med en uppgift. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | Den specifika platsen i ett dokument i en hyperlänk som är associerad med en uppgift. |
| [ID](#ID) | Positionsidentifieraren för en uppgift inom listan över uppgifter. |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | Bestämmer om schemaläggningen av uppgiften tar hänsyn till de resursernas kalendrar som är tilldelade uppgiften. |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | Anger om varningsindikatorn för schemakonflikt ska döljas i Microsoft Project. |
| [IS_ACTIVE](#IS-ACTIVE) | Bestämmer om en uppgift är aktiv. |
| [IS_CRITICAL](#IS-CRITICAL) | Bestämmer om en uppgift ligger på den kritiska vägen. |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | Bestämmer om schemaläggningen för uppgiften är insatsdriven schemaläggning. |
| [IS_ESTIMATED](#IS-ESTIMATED) | Bestämmer om en uppgift är uppskattad. |
| [IS_EXPANDED](#IS-EXPANDED) | Bestämmer om en samlingsuppgift är expanderad eller inte i GanttChart-vyn. |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | Bestämmer om en uppgift är extern. |
| [IS_MANUAL](#IS-MANUAL) | Bestämmer om en uppgift är manuellt schemalagd. |
| [IS_MARKED](#IS-MARKED) | Visar om en uppgift är markerad för vidare åtgärd eller någon form av identifiering. |
| [IS_MILESTONE](#IS-MILESTONE) | Bestämmer om en uppgift är en milstolpe. |
| [IS_NULL](#IS-NULL) | Bestämmer om en uppgift är en nulluppgift. |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | Anger om någon av de tilldelade resurserna på en uppgift är tilldelad mer arbete på uppgiften än vad som kan utföras inom normal arbetskapacitet. |
| [IS_PUBLISHED](#IS-PUBLISHED) | Bestämmer om den aktuella uppgiften ska publiceras till Project Server tillsammans med resten av projektet. |
| [IS_RECURRING](#IS-RECURRING) | Bestämmer om en uppgift är en del av en serie återkommande uppgifter. |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | Bestämmer om en uppgift kan återupptas. |
| [IS_ROLLUP](#IS-ROLLUP) | Bestämmer om information om deluppgiftens Gantt-staplar ska rullas upp till samlingsuppgiftens stapel. |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | Bestämmer om en uppgift är ett infogat projekt. |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | Bestämmer om ett delprojekt är skrivskyddat. |
| [IS_SUMMARY](#IS-SUMMARY) | Bestämmer om en uppgift är en samlingsuppgift. |
| [LATE_FINISH](#LATE-FINISH) | Det senaste datumet då en uppgift kan slutföras utan att fördröja projektets avslut. |
| [LATE_START](#LATE-START) | Det senaste datumet då en uppgift kan påbörjas utan att fördröja projektets avslut. |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | Bestämmer om resursutjämningsfunktionen kan orsaka delningar av återstående arbete på denna uppgift. |
| [LEVELING_DELAY](#LEVELING-DELAY) | Den tid som en uppgift ska försenas från sitt tidiga startdatum på grund av resursutjämning. |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | Bestämmer om utjämningsfunktionen kan fördröja och dela individuella tilldelningar för att lösa överallokeringar. |
| [MANUAL_DURATION](#MANUAL-DURATION) | Definierar manuellt schemalagd varaktighet för en uppgift. |
| [MANUAL_FINISH](#MANUAL-FINISH) | Definierar manuellt schemalagt slut för en uppgift. |
| [MANUAL_START](#MANUAL-START) | Definierar manuellt schemalagd start för en uppgift. |
| [NAME](#NAME) | Namnet på en uppgift. |
| [NOTES_RTF](#NOTES-RTF) | Textanteckningarna i RTF-format. |
| [NOTES_TEXT](#NOTES-TEXT) | Anteckningarnas rena text extraherad från RTF-data. |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | Utkastnivån för en uppgift. |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | Numret som representerar en uppgifts position i den hierarkiska strukturen. |
| [OVERTIME_COST](#OVERTIME-COST) | Den totala övertidskostnaden för en uppgift, för en resurs på alla tilldelade uppgifter, eller för en resursallokering. |
| [OVERTIME_WORK](#OVERTIME-WORK) | Mängden övertid som är schemalagd att utföras av alla resurser som är tilldelade en uppgift. |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | Den aktuella statusen för en uppgift, uttryckt som andelen av uppgiftens varaktighet som har slutförts. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | Den aktuella statusen för en uppgift uttryckt som andelen av arbetet som har slutförts. |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | Procentvärde för slutfört arbete som kan användas som ett alternativ för att beräkna budgeterad kostnad för utfört arbete (BCWP). |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | Slutdatumet för en uppgift som det var innan resurshantering utfördes. |
| [PRELEVELED_START](#PRELEVELED-START) | Startdatumet för en uppgift som det var innan resurshantering utfördes. |
| [PRIORITY](#PRIORITY) | Vikten som tilldelas en uppgift, vilket i sin tur indikerar hur lätt en uppgift eller tilldelning kan fördröjas eller delas upp under resurshantering. |
| [REGULAR_WORK](#REGULAR-WORK) | Den totala mängden icke-övertidsarbete som är schemalagt att utföras av resurser. |
| [REMAINING_COST](#REMAINING-COST) | Den återstående schemalagda kostnaden som kommer att uppstå vid slutförandet av det återstående schemalagda arbetet. |
| [REMAINING_DURATION](#REMAINING-DURATION) | Den tid som krävs för att slutföra den ofullständiga delen av en uppgift. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | Den återstående schemalagda övertidskostnaden för en uppgift. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | Mängden återstående schemalagda övertidstid. |
| [REMAINING_WORK](#REMAINING-WORK) | Den tid som fortfarande krävs för att slutföra en uppgift eller en uppgiftsuppsättning. |
| [RESUME](#RESUME) | Datumet då den återstående delen av en uppgift är schemalagd att återupptas efter att något framsteg har registrerats. |
| [START](#START) | Det schemalagda startdatumet för en uppgift. |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | Varaktigheten (i sekunder) mellan tidig start och sen start. |
| [START_TEXT](#START-TEXT) | Returnerar uppgiftens starttext. |
| [START_VARIANCE](#START-VARIANCE) | Tiden som representerar skillnaden mellan ett baslinjestartdatum för en uppgift eller tilldelning och dess aktuella schemalagda startdatum. |
| [STATUS_MANAGER](#STATUS-MANAGER) | Namnet på företagets resurs som ska ta emot statusuppdateringar för den aktuella uppgiften från resurser. |
| [STOP](#STOP) | Datumet som representerar slutet på den faktiska delen av en uppgift. |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | Källplatsen för ett delprojekt. |
| [SV](#SV) | Den intjänade värdeplanens avvikelse fram till projektets statusdatum. |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | Den tid som en uppgifts slutdatum kan fördröjas utan att fördröja projektets slutdatum. |
| [TYPE](#TYPE) | Typen av en uppgift. |
| [UID](#UID) | Det unika ID:t för en uppgift. |
| [WARNING](#WARNING) | Representerar flaggan som indikerar att uppgiften har schemaläggningsavvikelser. |
| [WBS](#WBS) | Arbetsnedbrytningsstruktur (WBS)-koder. |
| [WBS_LEVEL](#WBS-LEVEL) | Den högst till höger WBS-nivån för en uppgift. |
| [WORK](#WORK) | Den totala tid som är schemalagd för en uppgift för alla tilldelade resurser. |
| [WORK_VARIANCE](#WORK-VARIANCE) | Skillnaden mellan baslinjearbete för en uppgift och det för närvarande schemalagda arbetet. |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Byte> ACTIVITY_ID
```


Representerar aktivitets‑ID‑fältet – en uppgifts unika identifierare som används av Primavera. (gäller endast Primavera‑projekt).

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Kostnader som uppkommit för arbete som redan utförts av resurser på deras uppgifter, tillsammans med eventuella andra registrerade kostnader som är kopplade till uppgiften.

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Byte> ACTUAL_DURATION
```


Tidsintervallet för faktiskt arbetstid för en uppgift, baserat på den schemalagda varaktigheten och aktuellt återstående arbete eller färdigställt procenttal.

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


Datumet då en uppgift slutfördes.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Kostnader som uppkommit för övertidsarbete som redan utförts på uppgifter av tilldelade resurser.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


Den faktiska mängden övertidsarbete som redan utförts av resurser som tilldelats uppgifter.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


Varaktigheten under vilken faktiskt övertidsarbete är skyddat.

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


Datumet och tiden då en uppgift faktiskt påbörjades.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


Mängden arbete som redan har utförts av resurser som tilldelats uppgifter.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


Varaktigheten under vilken faktiskt arbete är skyddat.

--------------------

Läsning stöds endast för XML-format.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


Kostnader som uppkommit för arbete som redan utförts på en uppgift, fram till projektets statusdatum eller dagens datum.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


Det kumulativa värdet av uppgiftens färdigställt procenttal multiplicerat med de tidsfasade grundkostnaderna.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


De kumulativa tidsfasade grundkostnaderna fram till statusdatumet eller dagens datum.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Budgetkostnader för budgetkostnadsresurser. Budgetresurser tilldelas endast till projektets sammanfattningsuppgift.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


Budgetarbete för budgetarbete och materialresurser. Budgetresurser tilldelas endast till projektets sammanfattningsuppgift.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


Uppgiftens kalender.

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Byte> COMMITMENT_FINISH
```


Slutdatumet för en leverans.

--------------------

Läsning stöds endast för XML-format.

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Byte> COMMITMENT_START
```


Startdatumet för en leverans.

--------------------

Läsning stöds endast för XML-format.

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Byte> COMMITMENT_TYPE
```


Bestämmer om en uppgift har en associerad leverans eller ett beroende av en associerad leverans.

--------------------

Läsning stöds endast för XML-format.

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Byte> CONSTRAINT_DATE
```


Det specifika datumet som är associerat med begränsningstypen.

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Byte> CONSTRAINT_TYPE
```


Tillhandahåller val för vilken typ av begränsning som kan tillämpas vid schemaläggning av en uppgift.

### CONTACT {#CONTACT}
```
public static final Key<String,Byte> CONTACT
```


Namnet på den person som ansvarar för en uppgift.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


Den totala schemalagda eller beräknade kostnaden för en uppgift baserad på kostnader som redan uppkommit för arbete utfört av resurser som tilldelats uppgifterna, samt de kostnader som planeras för återstående arbete.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


Skillnaden mellan grundkostnaden och total kostnad för en uppgift, resurs eller tilldelning.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


Datumet då en uppgift skapades.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


Skillnaden mellan baslinjekostnad och total kostnad för en uppgift. Kostnadsavvikelse = Kostnad - Baslinjekostnad

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Byte> DEADLINE
```


Ett måldatum som visar när en uppgift ska slutföras.

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Byte> DISPLAY_AS_SUMMARY
```


Bestämmer om uppgiften ska visas som en sammanfattningsuppgift.

--------------------

Läsning stöds endast för XML-format.

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Byte> DISPLAY_ON_TIMELINE
```


Anger om en uppgift ska visas i en tidslinjevy.

### DURATION {#DURATION}
```
public static final Key<Duration,Byte> DURATION
```


Den totala perioden av aktiv arbetstid för en uppgift som anges eller beräknas av Microsoft Project baserat på startdatum, slutdatum, kalendrar och andra schemaläggningsfaktorer.

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Byte> DURATION_TEXT
```


Returnerar uppgiftens varaktighetstext.

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Byte> DURATION_VARIANCE
```


Skillnaden mellan grundlinjens varaktighet för en uppgift och den totala varaktigheten (aktuella uppskattningen) för en uppgift.

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Byte> EARLY_FINISH
```


Det tidigaste datumet då en uppgift eventuellt kan slutföras, baserat på tidiga slutdatum för föregående och efterföljande uppgifter, andra begränsningar och eventuell nivåfördröjning.

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Byte> EARLY_START
```


Det tidigaste datumet då en uppgift eventuellt kan påbörjas, baserat på tidiga startdatum för föregående och efterföljande uppgifter och andra begränsningar.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


Bestämmer om fältet % färdig eller Fysiskt % färdig ska användas för att beräkna budgeterad kostnad för utfört arbete (BCWP).

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Byte> EXTERNAL_ID
```


Om en uppgift är en extern uppgift innehåller den uppgiftens externa ID.

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Byte> EXTERNAL_TASK_PROJECT
```


Källplatsen och uppgiftsidentifieraren för en extern uppgift.

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Byte> EXTERNAL_UID
```


Innehåller den externa uppgiftens unika identifierare när uppgiften är extern.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


Det planerade slutdatumet för en uppgift.

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FINISH_SLACK_TIME_SPAN
```


Varaktigheten (i sekunder) mellan tidigt slut och sent slut datum.

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Byte> FINISH_TEXT
```


Returnerar uppgiftens slutttext.

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


Tiden som representerar skillnaden mellan grundlinjens slutdatum för en uppgift eller tilldelning och dess aktuella slutdatum.

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Byte> FIXED_COST
```


Visar eventuella kostnader för icke-resursuppgifter.

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> FIXED_COST_ACCRUAL
```


Bestämmer val för hur och när fasta kostnader ska debiteras eller bokföras till en uppgifts kostnad.

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FREE_SLACK_TIME_SPAN
```


Tiden (i sekunder) som en uppgift kan fördröjas utan att fördröja några efterföljande uppgifter.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


De genererade unika identifieringskoderna för en uppgift.

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Byte> HAS_OVERALLOCATED_RESOURCE
```


Indikerar om uppgiften har en resurs tilldelad som har mer arbete på tilldelade uppgifter än vad som kan slutföras inom normal arbetskapacitet.

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Byte> HIDE_BAR
```


Bestämmer om Gantt-stapeln för en uppgift är dold när den visas i Microsoft Project.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


Titeln eller förklarande text för en hyperlänk som är associerad med en uppgift.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


Adressen för en hyperlänk som är associerad med en uppgift.

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


Positionsidentifieraren för en uppgift inom listan över uppgifter.

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Byte> IGNORE_RESOURCE_CALENDAR
```


Bestämmer om schemaläggningen av uppgiften tar hänsyn till de resursernas kalendrar som är tilldelade uppgiften.

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Byte> IGNORE_WARNINGS
```


Anger om varningsindikatorn för schemakonflikt ska döljas i Microsoft Project.

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Byte> IS_ACTIVE
```


Bestämmer om en uppgift är aktiv. Inaktiva uppgifter påverkar inte längre andra uppgifter eller det övergripande projektschemat.

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Byte> IS_CRITICAL
```


Bestämmer om en uppgift ligger på den kritiska vägen.

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> IS_EFFORT_DRIVEN
```


Bestämmer om schemaläggningen för uppgiften är insatsdriven schemaläggning.

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Byte> IS_ESTIMATED
```


Bestämmer om en uppgift är uppskattad.

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Byte> IS_EXPANDED
```


Bestämmer om en samlingsuppgift är expanderad eller inte i GanttChart-vyn.

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Byte> IS_EXTERNAL_TASK
```


Bestämmer om en uppgift är extern.

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Byte> IS_MANUAL
```


Bestämmer om en uppgift är manuellt schemalagd.

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Byte> IS_MARKED
```


Visar om en uppgift är markerad för vidare åtgärd eller någon form av identifiering.

--------------------

Gäller endast mpp‑filformat.

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Byte> IS_MILESTONE
```


Bestämmer om en uppgift är en milstolpe.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Bestämmer om en uppgift är en nulluppgift.

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Byte> IS_OVERALLOCATED
```


Anger om någon av de tilldelade resurserna på en uppgift är tilldelad mer arbete på uppgiften än vad som kan utföras inom normal arbetskapacitet.

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Byte> IS_PUBLISHED
```


Bestämmer om den aktuella uppgiften ska publiceras till Project Server tillsammans med resten av projektet.

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Byte> IS_RECURRING
```


Bestämmer om en uppgift är en del av en serie återkommande uppgifter.

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Byte> IS_RESUME_VALID
```


Bestämmer om en uppgift kan återupptas.

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Byte> IS_ROLLUP
```


Bestämmer om information om deluppgiftens Gantt-staplar ska rullas upp till samlingsuppgiftens stapel.

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Byte> IS_SUBPROJECT
```


Bestämmer om en uppgift är ett infogat projekt.

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Byte> IS_SUBPROJECT_READ_ONLY
```


Bestämmer om ett delprojekt är skrivskyddat.

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Byte> IS_SUMMARY
```


Bestämmer om en uppgift är en samlingsuppgift.

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Byte> LATE_FINISH
```


Det senaste datumet då en uppgift kan slutföras utan att fördröja projektets avslut.

### LATE_START {#LATE-START}
```
public static final Key<Date,Byte> LATE_START
```


Det senaste datumet då en uppgift kan påbörjas utan att fördröja projektets avslut.

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Byte> LEVELING_CAN_SPLIT
```


Bestämmer om resursutjämningsfunktionen kan orsaka delningar av återstående arbete på denna uppgift.

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


Den tid som en uppgift ska försenas från sitt tidiga startdatum på grund av resursutjämning.

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Byte> LEVEL_ASSIGNMENTS
```


Bestämmer om utjämningsfunktionen kan fördröja och dela individuella tilldelningar för att lösa överallokeringar.

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Byte> MANUAL_DURATION
```


Definierar manuellt schemalagd varaktighet för en uppgift.

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Byte> MANUAL_FINISH
```


Definierar manuellt schemalagt slut för en uppgift.

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Byte> MANUAL_START
```


Definierar manuellt schemalagd start för en uppgift.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


Namnet på en uppgift.

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

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Byte> OUTLINE_LEVEL
```


Utkastnivån för en uppgift.

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Byte> OUTLINE_NUMBER
```


Numret som representerar en uppgifts position i den hierarkiska strukturen.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


Den totala övertidskostnaden för en uppgift, för en resurs på alla tilldelade uppgifter, eller för en resursallokering.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


Mängden övertid som är schemalagd att utföras av alla resurser som är tilldelade en uppgift.

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_COMPLETE
```


Den aktuella statusen för en uppgift, uttryckt som andelen av uppgiftens varaktighet som har slutförts.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


Den aktuella statusen för en uppgift uttryckt som andelen av arbetet som har slutförts.

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PHYSICAL_PERCENT_COMPLETE
```


Procentvärde för slutfört arbete som kan användas som ett alternativ för att beräkna budgeterad kostnad för utfört arbete (BCWP).

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Byte> PRELEVELED_FINISH
```


Slutdatumet för en uppgift som det var innan resurshantering utfördes.

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Byte> PRELEVELED_START
```


Startdatumet för en uppgift som det var innan resurshantering utfördes.

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Byte> PRIORITY
```


Vikten som tilldelas en uppgift, vilket i sin tur indikerar hur lätt en uppgift eller tilldelning kan fördröjas eller delas upp under resurshantering.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


Den totala mängden icke-övertidsarbete som är schemalagt att utföras av resurser.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


Den återstående schemalagda kostnaden som kommer att uppstå vid slutförandet av det återstående schemalagda arbetet.

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Byte> REMAINING_DURATION
```


Den tid som krävs för att slutföra den ofullständiga delen av en uppgift.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


Den återstående schemalagda övertidskostnaden för en uppgift.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


Mängden återstående schemalagda övertidstid.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


Den tid som fortfarande krävs för att slutföra en uppgift eller en uppgiftsuppsättning.

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


Datumet då den återstående delen av en uppgift är schemalagd att återupptas efter att något framsteg har registrerats.

### START {#START}
```
public static final Key<Date,Byte> START
```


Det schemalagda startdatumet för en uppgift.

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> START_SLACK_TIME_SPAN
```


Varaktigheten (i sekunder) mellan tidig start och sen start.

### START_TEXT {#START-TEXT}
```
public static final Key<String,Byte> START_TEXT
```


Returnerar uppgiftens starttext.

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


Tiden som representerar skillnaden mellan ett baslinjestartdatum för en uppgift eller tilldelning och dess aktuella schemalagda startdatum.

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Byte> STATUS_MANAGER
```


Namnet på företagets resurs som ska ta emot statusuppdateringar för den aktuella uppgiften från resurser.

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


Datumet som representerar slutet på den faktiska delen av en uppgift.

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Byte> SUBPROJECT_NAME
```


Källplatsen för ett delprojekt.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


Den intjänade värdeschematavvikelsen fram till projektets statusdatum. Schematavvikelse (SV) är skillnaden mellan BCWP och BCWS.

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> TOTAL_SLACK_TIME_SPAN
```


Den tid som en uppgifts slutdatum kan fördröjas utan att fördröja projektets slutdatum.

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


Typen av en uppgift.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


Det unika ID:t för en uppgift.

### WARNING {#WARNING}
```
public static final Key<Boolean,Byte> WARNING
```


Representerar flaggan som indikerar att uppgiften har schemaläggningsavvikelser.

### WBS {#WBS}
```
public static final Key<String,Byte> WBS
```


Arbetsnedbrytningsstruktur (WBS)-koder.

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Byte> WBS_LEVEL
```


Den högst till höger WBS-nivån för en uppgift.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


Den totala tid som är schemalagd för en uppgift för alla tilldelade resurser.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


Skillnaden mellan baslinjearbete för en uppgift och det för närvarande schemalagda arbetet.

