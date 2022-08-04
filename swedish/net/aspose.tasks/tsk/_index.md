---
title: Tsk
second_title: Aspose.Tasks för .NET API-referens
description: Representerar egenskaper förTask./task objekt.
type: docs
weight: 2290
url: /sv/net/aspose.tasks/tsk/
---
## Tsk class

Representerar egenskaper för[`Task`](../task) objekt.

```csharp
public static class Tsk
```

## Fält

| namn | Beskrivning |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid) | Representerar aktivitets-id-fält - en uppgifts unika identifierare som används av Primavera. (gäller endast Primavera-projekt). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost) | Kostnader för arbete som redan utförts av resurser på deras uppgifter, tillsammans med alla andra registrerade kostnader som är associerade med uppgiften. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration) | Spännvidden av faktisk arbetstid för en uppgift, baserat på schemalagd varaktighet och aktuellt återstående arbete eller procent slutfört. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish) | Datumet då en uppgift slutfördes. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost) | Kostnader för övertidsarbete som redan utförts på uppgifter av tilldelade resurser. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework) | Den faktiska mängden övertidsarbete som redan utförts av resurser som tilldelats uppgifter. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected) | Den varaktighet genom vilken faktisk övertidsarbete skyddas.  Läsning stöds endast för XML-format. [`Duration`](./duration) typ. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart) | Datum och tid då en uppgift faktiskt började. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork) | Mängden arbete som redan har utförts av resurser som tilldelats uppgifter. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected) | Varaktigheten genom vilken det faktiska arbetet är skyddat.  Läsning stöds endast för XML-format. [`Duration`](./duration) typ. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp) | Kostnader för arbete som redan utförts på en uppgift, fram till projektets statusdatum eller dagens datum. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp) | Det kumulativa värdet av uppgiftens procentuella slutförda multiplicerat med de tidsfasade baslinjekostnaderna. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws) | De ackumulerade tidsfasade baslinjekostnaderna fram till statusdatumet eller dagens datum. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost) | Budgetkostnader för budgetkostnadsresurser. Budgetresurser tilldelas endast projektsammanfattningsuppgiften. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork) | Budgetarbete för budgetarbete och materialresurser. Budgetresurser tilldelas endast projektsammanfattningsuppgiften. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar) | Uppgiftskalendern. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish) | Slutdatum för en leverans.  Läsning stöds endast för XML-format. DateTime typ. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart) | Startdatum för en leverans.  Läsning stöds endast för XML-format. DateTime typ. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype) | Bestämmer om en uppgift har en associerad leverans eller ett beroende av en associerad leverans.  Läsning stöds endast för XML-format. Int32 typ. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate) | Det specifika datumet som är kopplat till begränsningstypen. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype) | Ger val för vilken typ av begränsning som kan tillämpas för att schemalägga en uppgift. |
| static readonly [Contact](../../aspose.tasks/tsk/contact) | Namnet på en person som ansvarar för en uppgift. |
| static readonly [Cost](../../aspose.tasks/tsk/cost) | Den totala schemalagda eller beräknade kostnaden för en uppgift baserat på kostnader som redan har uppkommit för arbete som utförts av resurser som tilldelats uppgifterna, utöver de planerade kostnaderna för det återstående arbetet. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance) | Skillnaden mellan baskostnaden och totalkostnaden för en uppgift, resurs eller uppdrag. |
| static readonly [Created](../../aspose.tasks/tsk/created) | Datumet då en uppgift skapades. |
| static readonly [CV](../../aspose.tasks/tsk/cv) | Skillnaden mellan baskostnaden och totalkostnaden för en uppgift. Kostnadsvarians = Kostnad - Baslinjekostnad |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline) | Ett måldatum som anger när en uppgift ska slutföras. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary) | Bestämmer om uppgiften ska visas som en sammanfattningsuppgift.  Läsning stöds endast för XML-format. Boolean typ. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline) | Anger om en uppgift ska visas i en tidslinjevy. |
| static readonly [Duration](../../aspose.tasks/tsk/duration) | Det totala intervallet för aktiv arbetstid för en uppgift som den har angetts eller beräknats av Microsoft Project baserat på startdatum, slutdatum, kalendrar och andra schemaläggningsfaktorer. |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat) | Uppgiftens varaktighetsformat. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext) | Returnerar uppgiftens varaktighetstext. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance) | Skillnaden mellan baslinjevaraktigheten för en uppgift och den totala varaktigheten (nuvarande uppskattning) för en uppgift. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish) | Det tidigaste datumet som en uppgift skulle kunna slutföras, baserat på tidiga slutdatum för föregångare och efterföljande uppgifter, andra begränsningar och eventuell utjämningsfördröjning. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart) | Det tidigaste datumet då en uppgift möjligen skulle kunna börja, baserat på de tidiga startdatumen för föregångare och efterföljande uppgifter och andra begränsningar. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod) | Bestämmer om fältet % färdigt eller fysiskt % färdigställt ska användas för att beräkna budgeterad kostnad för utfört arbete (BCWP). |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid) | Om en uppgift är en extern uppgift innehåller den uppgiftens externa Id. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject) | Källplatsen och uppgiftsidentifieraren för en extern uppgift. |
| static readonly [Finish](../../aspose.tasks/tsk/finish) | Det schemalagda slutdatumet för en uppgift. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan) | Längden mellan datum för tidig målgång och sen målgång. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext) | Returnerar uppgiftens sluttext. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance) | Tiden som representerar skillnaden mellan baslinjens slutdatum för en uppgift eller uppgift och dess nuvarande slutdatum. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost) | Visar alla utgifter som inte är resursuppgifter. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual) | Bestämmer val för hur och när fasta kostnader ska debiteras, eller periodiseras, till kostnaden för en uppgift. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan) | Tiden som en uppgift kan försenas utan att försena några efterföljande uppgifter. |
| static readonly [Guid](../../aspose.tasks/tsk/guid) | De genererade unika identifikationskoderna för en uppgift. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource) | Indikerar om uppgiften har en resurs tilldelad som har mer arbete på tilldelade uppgifter än vad som kan slutföras inom normal arbetskapacitet. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar) | Bestämmer om Gantt-fältet för en uppgift är dold när det visas i Microsoft Project. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink) | Titeln eller förklarande texten för en hyperlänk kopplad till en uppgift. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress) | Adressen för en hyperlänk kopplad till en uppgift. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress) | Den specifika platsen i ett dokument i en hyperlänk kopplad till en uppgift. |
| static readonly [Id](../../aspose.tasks/tsk/id) | Positionsidentifieraren för en uppgift i listan med uppgifter. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar) | Bestämmer om schemaläggningen av uppgiften tar hänsyn till kalendrarna för de resurser som tilldelats uppgiften. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings) | Indikerar om varningsindikatorn för schemakonflikt ska döljas i Microsoft Project. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive) | Bestämmer om en uppgift är aktiv. Inaktiva uppgifter påverkar inte längre andra uppgifter eller det övergripande projektschemat. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical) | Bestämmer om en uppgift är på den kritiska vägen. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven) | Avgör om schemaläggningen för uppgiften är ansträngningsdriven schemaläggning. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated) | Bestämmer om en uppgift uppskattas. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded) | Bestämmer om en sammanfattningsuppgift utökas eller inte i GanttChart-vyn. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask) | Bestämmer om en uppgift är extern. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual) | Bestämmer om en uppgift är manuellt schemalagd. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked) | Visar om en uppgift är markerad för ytterligare åtgärd eller identifiering av något slag. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone) | Avgör om en uppgift är en milstolpe. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull) | Avgör om en uppgift är en nolluppgift. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated) | Indikerar om någon av de tilldelade resurserna för en uppgift är tilldelad mer arbete på uppgiften än vad som kan utföras med normal arbetskapacitet. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished) | Bestämmer om den aktuella uppgiften ska publiceras till Project Server med resten av projektet. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring) | Bestämmer om en uppgift är en del av en serie återkommande uppgifter. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid) | Avgör om en uppgift kan återupptas. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup) | Bestämmer om information om deluppgiftens Gantt-staplar kommer att rullas upp till den sammanfattande aktivitetsfältet. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject) | Avgör om en uppgift är ett infogat projekt. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly) | Bestämmer om ett delprojekt är skrivskyddat. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary) | Bestämmer om en uppgift är en sammanfattningsuppgift. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish) | Det senaste datumet som en uppgift kan avslutas utan att försena projektets slut. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart) | Det senaste datumet då en uppgift kan starta utan att fördröja projektets slut. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments) | Bestämmer om utjämningsfunktionen kan fördröja och dela upp individuella tilldelningar för att lösa över tilldelningar. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit) | Bestämmer om resursutjämningsfunktionen kan orsaka uppdelningar på återstående arbete med denna uppgift. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay) | Tiden då en uppgift ska försenas från dess tidiga startdatum på grund av resursutjämning. |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat) | Formatet för att uttrycka varaktigheten av en fördröjning. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration) | Definierar manuellt schemalagd varaktighet för en uppgift. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish) | Definierar manuellt schemalagd slutföring av en uppgift. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart) | Definierar manuellt schemalagd start av en uppgift. |
| static readonly [Name](../../aspose.tasks/tsk/name) | En uppgifts namn. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf) | Textanteckningarna i RTF-format. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext) | Notes' oformaterad text extraherad från RTF-data. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel) | Konturnivån för en uppgift. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber) | Siffran som representerar en uppgifts position i den hierarkiska konturstrukturen. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost) | Den totala övertidskostnaden för en uppgift, för en resurs på alla tilldelade uppgifter eller för en resurstilldelning. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework) | Mängden övertid som är planerad att utföras av alla resurser som tilldelats en uppgift. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete) | Aktuell status för en uppgift, uttryckt som procentandelen av uppgiftens varaktighet som har slutförts. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete) | Aktuell status för en uppgift uttryckt som den procentuella andelen arbete som har slutförts. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete) | Procent fullständigt värde som kan användas som ett alternativ för att beräkna budgeterad kostnad för utfört arbete (BCWP). |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish) | Slutdatumet för en uppgift som det var innan resursutjämningen gjordes. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart) | Startdatumet för en uppgift som det var innan resursutjämningen gjordes. |
| static readonly [Priority](../../aspose.tasks/tsk/priority) | Graden av vikt som ges till en uppgift, vilket i sin tur indikerar hur lätt en uppgift eller uppdrag kan försenas eller delas upp under resursutjämning. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork) | Den totala mängden icke övertidsarbete som planeras att utföras av resurser. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost) | Den återstående schemalagda kostnaden som kommer att uppstå för att slutföra det återstående schemalagda arbetet. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration) | Den tid som krävs för att slutföra den oavslutade delen av en uppgift. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost) | Den återstående schemalagda övertidskostnaden för en uppgift. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework) | Mängden återstående schemalagd övertidstid. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork) | Den tid som fortfarande krävs för att slutföra en uppgift eller en uppsättning uppgifter. |
| static readonly [Resume](../../aspose.tasks/tsk/resume) | Datumet då den återstående delen av en uppgift är schemalagd att återupptas efter att ha angett något förlopp. |
| static readonly [Start](../../aspose.tasks/tsk/start) | Det schemalagda startdatumet för en uppgift. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan) | Längden mellan datumet för tidig start och sen start. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext) | Returnerar uppgiftens starttext. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance) | Den tid som representerar skillnaden mellan ett baslinjestartdatum för en uppgift eller uppgift och dess för närvarande schemalagda startdatum. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager) | Namnet på företagsresursen som ska ta emot statusuppdateringar för den aktuella uppgiften från resurser. |
| static readonly [Stop](../../aspose.tasks/tsk/stop) | Datumet som representerar slutet av den faktiska delen av en uppgift. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname) | Källplatsen för ett delprojekt. |
| static readonly [SV](../../aspose.tasks/tsk/sv) | Schemavariansen för intjänat värde, till och med projektets statusdatum. Schemavarians (SV) är skillnaden mellan BCWP och BCWS. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan) | Tiden då en uppgifts slutdatum kan försenas utan att försena projektets slutdatum. |
| static readonly [Type](../../aspose.tasks/tsk/type) | Typen av en uppgift. |
| static readonly [Uid](../../aspose.tasks/tsk/uid) | Det unika ID:t för en uppgift. |
| static readonly [Warning](../../aspose.tasks/tsk/warning) | Representerar flaggan som indikerar att uppgiften har schemaavvikelser. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs) | Koder för arbetsuppdelningsstruktur (WBS). |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel) | WBS-nivån längst till höger för en uppgift. |
| static readonly [Work](../../aspose.tasks/tsk/work) | Den totala tiden som schemalagts för en uppgift för alla tilldelade resurser. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance) | Skillnaden mellan baslinjearbete för en uppgift och det för närvarande schemalagda arbetet. |

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
