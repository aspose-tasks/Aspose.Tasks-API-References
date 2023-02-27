---
title: Class Tsk
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.Tsk classe. Rappresenta le proprietà diTask oggetto.
type: docs
weight: 2310
url: /it/net/aspose.tasks/tsk/
---
## Tsk class

Rappresenta le proprietà di[`Task`](../task/) oggetto.

```csharp
public static class Tsk
```

## Campi

| Nome | Descrizione |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | Rappresenta il campo ID attività: l'identificatore univoco di un'attività utilizzato da Primavera. (applicabile solo ai progetti Primavera). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | Costi sostenuti per il lavoro già eseguito dalle risorse sulle loro attività, insieme a qualsiasi altro costo registrato associato all'attività. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | L'intervallo di tempo di lavoro effettivo per un'attività, in base alla durata pianificata e al lavoro rimanente corrente o alla percentuale di completamento. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | La data in cui è stata completata un'attività. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | Costi sostenuti per lavoro straordinario già svolto su incarichi dalle risorse assegnate. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | La quantità effettiva di lavoro straordinario già svolto dalle risorse assegnate alle attività. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | La durata durante la quale il lavoro straordinario effettivo è protetto. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | La data e l'ora di inizio effettivo di un'attività. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | La quantità di lavoro già svolto dalle risorse assegnate alle attività. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | La durata durante la quale il lavoro effettivo è protetto. Lettura supportata solo per il formato XML. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | Costi sostenuti per il lavoro già svolto su un'attività, fino alla data dello stato del progetto o alla data odierna. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | Il valore cumulativo della percentuale di completamento dell'attività moltiplicato per i costi di base in scala cronologica. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | I costi di base cumulativi per fasi temporali fino alla data stato o alla data odierna. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | Costi a budget per le risorse dei costi a budget. Le risorse di budget vengono assegnate solo all'attività di riepilogo del progetto. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | Lavoro di bilancio per lavoro di bilancio e risorse materiali. Le risorse di budget vengono assegnate solo all'attività di riepilogo del progetto. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | Il calendario delle attività. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | La data di fine di una consegna.  Lettura supportata solo per il formato XML. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | La data di inizio di una consegna. Lettura supportata solo per il formato XML. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | Determina se un'attività ha una consegna associata o una dipendenza da una consegna associata.  Lettura supportata solo per il formato XML. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | La data specifica associata al tipo di vincolo. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | Fornisce scelte per il tipo di vincolo che può essere applicato per la pianificazione di un'attività. |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | Il nome di una persona responsabile di un'attività. |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | Il costo totale pianificato o previsto per un'attività in base ai costi già sostenuti per il lavoro eseguito dalle risorse assegnate alle attività, oltre ai costi pianificati per il lavoro rimanente. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | La differenza tra il costo previsto e il costo totale per un'attività, una risorsa o un'assegnazione. |
| static readonly [Created](../../aspose.tasks/tsk/created/) | La data in cui è stata creata un'attività. |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | La differenza tra il costo previsto e il costo totale per un'attività. Varianza costo = Costo - Costo previsto |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | Una data di destinazione che indica quando un'attività deve essere completata. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | Determina se l'attività deve essere visualizzata come attività di riepilogo. Lettura supportata solo per il formato XML. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | Specifica se un'attività deve essere visualizzata su una visualizzazione della sequenza temporale. |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | L'intervallo totale dell'orario di lavoro attivo per un'attività immesso o calcolato da Microsoft Project in base alla data di inizio, alla data di fine, ai calendari e ad altri fattori di pianificazione. |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat/) | Formato durata attività. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | Restituisce il testo della durata dell'attività. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | La differenza tra la durata prevista di un'attività e la durata totale (stima corrente) di un'attività. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | La prima data in cui un'attività potrebbe finire, in base alle date di fine anticipata delle attività predecessore e successore, altri vincoli e qualsiasi ritardo di livellamento. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | La prima data in cui un'attività potrebbe iniziare, in base alle prime date di inizio delle attività predecessore e successore e altri vincoli. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | Determina se il campo % completamento o % fisico completamento deve essere utilizzato per calcolare il costo preventivato del lavoro svolto (BCWP). |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | Se un'attività è un'attività esterna, contiene l'ID esterno dell'attività. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | La posizione di origine e l'identificatore dell'attività di un'attività esterna. |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | Contiene l'identificatore univoco dell'attività esterna quando l'attività è esterna. |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | La data di fine pianificata di un'attività. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | La durata tra le date di fine anticipata e di fine ultimata. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | Restituisce il testo finale dell'attività. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | L'ora che rappresenta la differenza tra la data di fine prevista di un'attività o assegnazione e la data di fine corrente. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | Mostra eventuali spese per attività diverse dalle risorse. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | Determina le scelte relative a come e quando i costi fissi devono essere addebitati, o accumulati, al costo di un'attività. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | Il tempo in cui un'attività può essere ritardata senza ritardare le attività successive. |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | I codici di identificazione univoci generati per un'attività. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | Indica se all'attività è assegnata una risorsa che ha più lavoro sulle attività assegnate di quanto possa essere completato entro la normale capacità lavorativa. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | Determina se la barra di Gantt di un'attività è nascosta quando viene visualizzata in Microsoft Project. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | Il titolo o il testo esplicativo per un collegamento ipertestuale associato a un'attività. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | L'indirizzo di un collegamento ipertestuale associato a un'attività. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | La posizione specifica in un documento in un collegamento ipertestuale associato a un'attività. |
| static readonly [Id](../../aspose.tasks/tsk/id/) | L'identificatore di posizione di un'attività all'interno dell'elenco delle attività. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | Determina se la schedulazione dell'attività considera i calendari delle risorse assegnate all'attività. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | Indica se nascondere l'indicatore di avviso di conflitto di pianificazione in Microsoft Project. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | Determina se un'attività è attiva. Le attività inattive non influiscono più sulle altre attività o sulla pianificazione generale del progetto. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | Determina se un'attività si trova sul percorso critico. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | Determina se la pianificazione dell'attività è basata sullo sforzo. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | Determina se un'attività è stimata. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | Determina se un'attività di riepilogo è espansa o meno nella visualizzazione Diagramma di Gantt. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | Determina se un'attività è esterna. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | Determina se un'attività è pianificata manualmente. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | Mostra se un'attività è contrassegnata per ulteriori azioni o identificazione di qualche tipo. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | Determina se un'attività è una pietra miliare. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | Determina se un'attività è un'attività nulla. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | Indica se una qualsiasi delle risorse assegnate su un'attività è assegnata a più lavoro sull'attività rispetto a quanto può essere svolto con la normale capacità lavorativa. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | Determina se l'attività corrente deve essere pubblicata in Project Server con il resto del progetto. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | Determina se un'attività fa parte di una serie di attività ricorrenti. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | Determina se un'attività può essere ripresa. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | Determina se le informazioni sulle barre di Gantt delle attività secondarie verranno riportate nella barra delle attività di riepilogo. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | Determina se un'attività è un progetto inserito. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | Determina se un sottoprogetto è di sola lettura. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | Determina se un'attività è un'attività di riepilogo. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | L'ultima data in cui un'attività può terminare senza ritardare la fine del progetto. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | L'ultima data in cui un'attività può iniziare senza ritardare la fine del progetto. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | Determina se la funzione di livellamento può ritardare e suddividere singole assegnazioni per risolvere le assegnazioni in eccesso. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | Determina se la funzione di livellamento delle risorse può causare divisioni sul lavoro rimanente su questa attività. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | L'ora in cui un'attività deve essere ritardata rispetto alla data di inizio anticipata a causa del livellamento delle risorse. |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat/) | Il formato per esprimere la durata di un ritardo. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | Definisce la durata pianificata manualmente di un'attività. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | Definisce la fine pianificata manualmente di un'attività. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | Definisce l'avvio pianificato manualmente di un'attività. |
| static readonly [Name](../../aspose.tasks/tsk/name/) | Il nome di un'attività. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | Le note di testo in formato RTF. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | Testo in chiaro delle note estratto dai dati RTF. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | Il livello di struttura di un'attività. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | Il numero che rappresenta la posizione di un'attività nella struttura gerarchica del profilo. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | Il costo del lavoro straordinario totale per un'attività, per una risorsa su tutte le attività assegnate o per un'assegnazione di risorse. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | La quantità di straordinari programmati per essere eseguiti da tutte le risorse assegnate a un'attività. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | Lo stato corrente di un'attività, espresso come percentuale della durata dell'attività che è stata completata. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | Lo stato corrente di un'attività espresso come percentuale di lavoro che è stato completato. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | Valore percentuale di completamento che può essere utilizzato come alternativa per il calcolo del costo preventivato del lavoro svolto (BCWP). |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | La data di fine di un'attività com'era prima del completamento del livellamento delle risorse. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | La data di inizio di un'attività com'era prima che fosse eseguito il livellamento delle risorse. |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | Il livello di importanza attribuito a un'attività, che a sua volta indica la facilità con cui un'attività o un'assegnazione può essere ritardata o suddivisa durante il livellamento delle risorse. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | La quantità totale di lavoro non straordinario programmato per essere svolto dalle risorse. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | La spesa programmata rimanente che verrà sostenuta per completare il lavoro programmato rimanente. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | Il tempo necessario per completare la parte non completata di un'attività. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | La spesa per gli straordinari pianificati rimanenti per un'attività. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | La quantità di tempo straordinario rimanente programmato. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | Il tempo ancora necessario per completare un'attività o una serie di attività. |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | La data in cui è pianificata la ripresa della parte rimanente di un'attività dopo l'immissione di qualsiasi stato di avanzamento. |
| static readonly [Start](../../aspose.tasks/tsk/start/) | La data di inizio pianificata di un'attività. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | La durata tra le date di inizio anticipato e di inizio posticipato. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | Restituisce il testo iniziale dell'attività. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | L'ora che rappresenta la differenza tra la data di inizio prevista di un'attività o assegnazione e la data di inizio attualmente pianificata. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | Il nome della risorsa dell'organizzazione che deve ricevere gli aggiornamenti di stato per l'attività corrente dalle risorse. |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | La data che rappresenta la fine della parte effettiva di un'attività. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | Il percorso di origine di un sottoprogetto. |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | La varianza della schedulazione del valore realizzato, fino alla data dello stato del progetto. La varianza della schedulazione (SV) è la differenza tra il BCWP e il BCWS. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | L'ora in cui la data di fine di un'attività può essere ritardata senza ritardare la data di fine del progetto. |
| static readonly [Type](../../aspose.tasks/tsk/type/) | Il tipo di attività. |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | L'ID univoco di un'attività. |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | Rappresenta il flag che indica che l'attività presenta discrepanze nella pianificazione. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | Codici WBS (Work Breakdown Structure). |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | Il livello WBS più a destra di un'attività. |
| static readonly [Work](../../aspose.tasks/tsk/work/) | Il tempo totale pianificato per un'attività per tutte le risorse assegnate. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | La differenza tra il lavoro previsto di un'attività e il lavoro attualmente pianificato. |

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


