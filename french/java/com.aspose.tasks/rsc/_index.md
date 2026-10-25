---
title: "Rsc"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les propriétés prises en charge de l'objet Resource."
type: docs
weight: 271
url: /fr/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

Représente les propriétés prises en charge de l'objet `Resource`.
## Champs

| Champ | Description |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | Détermine comment et quand les coûts standard et supplémentaires des ressources doivent être facturés ou imputés au coût d'une tâche. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | Le GUID Active Directory d'une ressource. |
| [ACTUAL_COST](#ACTUAL-COST) | Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches, ainsi que tous les autres coûts enregistrés associés à la tâche. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Coûts engagés pour le travail supplémentaire déjà effectué sur les tâches par les ressources assignées. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | Le montant réel du travail supplémentaire déjà effectué par la ressource assignée aux tâches. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | Le montant de travail à travers lequel le travail supplémentaire réel est protégé. |
| [ACTUAL_WORK](#ACTUAL-WORK) | Le montant de travail déjà effectué par la ressource assignée aux tâches. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | Le montant de travail à travers lequel le travail réel est protégé. |
| [ACWP](#ACWP) | Le coût réel d'un travail effectué par une ressource pour le projet à ce jour. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | Le nom du propriétaire d'une affectation. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | Le GUID du propriétaire d'une affectation. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | La date de début à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle. |
| [AVAILABLE_TO](#AVAILABLE-TO) | La date de fin à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle. |
| [BCWP](#BCWP) | Le coût budgété d'un travail effectué par une ressource pour le projet à ce jour. |
| [BCWS](#BCWS) | Le coût budgétaire d'un travail planifié pour une ressource. |
| [BOOKING_TYPE](#BOOKING-TYPE) | Le type de réservation d'une ressource. |
| [BUDGET_COST](#BUDGET-COST) | Coûts budgétaires pour les ressources à coût budgété. |
| [BUDGET_WORK](#BUDGET-WORK) | travail budgété pour le travail budgété et les ressources matérielles. |
| [CALENDAR](#CALENDAR) | Le calendrier d'une ressource. |
| [CAN_LEVEL](#CAN-LEVEL) | Détermine si le nivellement des ressources peut être effectué sur une ressource. |
| [CODE](#CODE) | Le code ou d'autres informations concernant une ressource. |
| [COST](#COST) | Le coût total planifié ou projeté pour une ressource, basé sur les coûts déjà engagés pour le travail effectué par les ressources assignées aux tâches, en plus des coûts prévus pour le travail restant. |
| [COST_CENTER](#COST-CENTER) | Indique à quel centre de coûts les coûts accumulés par la ressource doivent être imputés. |
| [COST_PER_USE](#COST-PER-USE) | Le coût qui s'accumule chaque fois qu'une ressource est utilisée. |
| [COST_VARIANCE](#COST-VARIANCE) | La différence entre le coût de référence et le coût total pour une ressource. |
| [CREATED](#CREATED) | La date et l'heure auxquelles une ressource a été ajoutée au projet. |
| [CV](#CV) | La variance du coût de la valeur acquise, jusqu'à la date d'état du projet. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | L'adresse e-mail d'une ressource. |
| [FINISH](#FINISH) | La date à laquelle une ressource est prévue pour terminer le travail sur toutes les tâches assignées. |
| [GROUP](#GROUP) | Le groupe auquel appartient une ressource. |
| [GUID](#GUID) | Contient le code d’identification unique généré pour la ressource. |
| [HYPERLINK](#HYPERLINK) | Le titre ou le texte explicatif d’un hyperlien associé à une ressource. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | L’adresse d’un hyperlien associé à une ressource. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | L’emplacement spécifique dans un document d’un hyperlien associé à une tâche. |
| [ID](#ID) | L’identifiant de position d’une ressource dans la liste des ressources. |
| [INACTIVE](#INACTIVE) | Détermine si une ressource a été rendue inactive par un utilisateur disposant de droits administratifs. |
| [INITIALS](#INITIALS) | Les initiales d’une ressource. |
| [IS_BUDGET](#IS-BUDGET) | Détermine si une ressource de travail, de matériel ou de coût est une ressource budgétaire. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | Détermine si une ressource est une ressource de coût. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | Indique si une ressource provient du pool de ressources d’entreprise (vrai) ou du pool de ressources local (faux). |
| [IS_GENERIC](#IS-GENERIC) | Détermine si une ressource est générique ou non. |
| [IS_NULL](#IS-NULL) | Détermine si une ressource est nulle. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | Indique si la ressource actuelle est une ressource d’équipe. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | L’unité de mesure pour la ressource matérielle. |
| [MAX_UNITS](#MAX-UNITS) | Le nombre maximal d’unités représentant la capacité maximale pour laquelle une ressource est disponible afin d’accomplir des tâches pendant la période actuelle. |
| [NAME](#NAME) | Le nom d’une ressource. |
| [NOTES_RTF](#NOTES-RTF) | Les notes texte au format RTF. |
| [NOTES_TEXT](#NOTES-TEXT) | Texte brut des notes extrait des données RTF. |
| [OVERALLOCATED](#OVERALLOCATED) | Indique si une ressource est affectée à plus de travail sur une tâche spécifique ou sur toutes les tâches que ce qui peut être accompli dans la capacité de travail normale. |
| [OVERTIME_COST](#OVERTIME-COST) | Le coût total des heures supplémentaires pour une ressource sur toutes les tâches assignées. |
| [OVERTIME_RATE](#OVERTIME-RATE) | Le taux de rémunération des heures supplémentaires effectuées par une ressource. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Les unités utilisées par Microsoft Project pour afficher le taux des heures supplémentaires. |
| [OVERTIME_WORK](#OVERTIME-WORK) | Le montant des heures supplémentaires prévu pour être effectué par une ressource sur une tâche et facturé aux taux des heures supplémentaires des ressources concernées. |
| [PEAK_UNITS](#PEAK-UNITS) | L'unité d'affectation maximale pour une ressource à tout moment pour toutes les tâches auxquelles la ressource est affectée. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | Le pourcentage de travail accompli sur toutes les tâches. |
| [PHONETICS](#PHONETICS) | L'orthographe phonétique du nom de la ressource. |
| [REGULAR_WORK](#REGULAR-WORK) | Le montant total du travail non supplémentaire prévu à être effectué par la ressource. |
| [REMAINING_COST](#REMAINING-COST) | La dépense prévue restante qui sera engagée pour terminer le travail prévu restant. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | La dépense supplémentaire prévue restante pour une ressource. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | Le montant du temps supplémentaire prévu restant. |
| [REMAINING_WORK](#REMAINING-WORK) | Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches. |
| [STANDARD_RATE](#STANDARD-RATE) | Le taux de rémunération pour le travail régulier, non supplémentaire, effectué par une ressource. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Les unités utilisées par Microsoft Project pour afficher le taux standard. |
| [START](#START) | La date à laquelle une ressource assignée est prévue pour commencer à travailler sur une tâche. |
| [SV](#SV) | L'écart de planification de la valeur acquise, jusqu'à la date d'état du projet. |
| [TYPE](#TYPE) | Le type d'une ressource. |
| [UID](#UID) | L'identifiant unique d'une ressource. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | Le compte NT associé à une ressource. |
| [WORK](#WORK) | Le montant total de temps prévu pour une ressource sur une tâche. |
| [WORKGROUP](#WORKGROUP) | Le type d'un groupe de travail auquel une ressource appartient. |
| [WORK_VARIANCE](#WORK-VARIANCE) | La différence entre le travail de référence d'une ressource et le travail actuellement prévu. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


Détermine comment et quand les coûts standard et supplémentaires des ressources doivent être facturés ou imputés au coût d'une tâche.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


Le GUID Active Directory d'une ressource.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches, ainsi que tous les autres coûts enregistrés associés à la tâche.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Coûts engagés pour le travail supplémentaire déjà effectué sur les tâches par les ressources assignées.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


Le montant réel du travail supplémentaire déjà effectué par la ressource assignée aux tâches.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


Le montant de travail à travers lequel le travail supplémentaire réel est protégé.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


Le montant de travail déjà effectué par la ressource assignée aux tâches.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


Le montant de travail à travers lequel le travail réel est protégé.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


Le coût réel d'un travail effectué par une ressource pour le projet à ce jour.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


Le nom du propriétaire d'une affectation.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


Le GUID du propriétaire d'une affectation.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


La date de début à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


La date de fin à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


Le coût budgété d'un travail effectué par une ressource pour le projet à ce jour.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


Le coût budgétaire d'un travail planifié pour une ressource.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


Le type de réservation d'une ressource.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Coûts budgétaires pour les ressources de coût budgétaire. Les ressources budgétaires sont affectées uniquement à la tâche de synthèse du projet.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


Travail budgété pour les ressources de travail budgété et matérielles. Les ressources budgétaires sont affectées uniquement à la tâche de synthèse du projet.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


Le calendrier d'une ressource.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


Détermine si le nivellement des ressources peut être effectué sur une ressource.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


Le code ou d'autres informations concernant une ressource.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


Le coût total planifié ou projeté pour une ressource, basé sur les coûts déjà engagés pour le travail effectué par les ressources assignées aux tâches, en plus des coûts prévus pour le travail restant.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


Indique à quel centre de coûts les coûts accumulés par la ressource doivent être imputés.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


Le coût qui s'accumule chaque fois qu'une ressource est utilisée.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


La différence entre le coût de référence et le coût total pour une ressource.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


La date et l'heure auxquelles une ressource a été ajoutée au projet.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


L'écart de coût de la valeur acquise, jusqu'à la date d'état du projet. CV est la différence entre le BCWP (coût budgété du travail effectué) de la tâche et l'ACWP (coût réel du travail effectué).

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


L'adresse e-mail d'une ressource.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


La date à laquelle une ressource est prévue pour terminer le travail sur toutes les tâches assignées.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


Le groupe auquel appartient une ressource.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


Contient le code d’identification unique généré pour la ressource.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


Le titre ou le texte explicatif d’un hyperlien associé à une ressource.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


L’adresse d’un hyperlien associé à une ressource.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


L’emplacement spécifique dans un document d’un hyperlien associé à une tâche.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


L’identifiant de position d’une ressource dans la liste des ressources.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


Détermine si une ressource a été rendue inactive par un utilisateur disposant de droits administratifs.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


Les initiales d’une ressource.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


Détermine si une ressource de travail, de matériel ou de coût est une ressource budgétaire.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


Détermine si une ressource est une ressource de coût.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


Indique si une ressource provient du pool de ressources d’entreprise (vrai) ou du pool de ressources local (faux).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


Détermine si une ressource est générique ou non.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Détermine si une ressource est nulle.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


Indique si la ressource actuelle est une ressource d’équipe.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


L’unité de mesure pour la ressource matérielle.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


Le nombre maximal d’unités représentant la capacité maximale pour laquelle une ressource est disponible afin d’accomplir des tâches pendant la période actuelle.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


Le nom d’une ressource.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


Les notes texte au format RTF.

--------------------

Pris en charge uniquement pour les formats MPP.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


Texte brut des notes extrait des données RTF.

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


Indique si une ressource est affectée à plus de travail sur une tâche spécifique ou sur toutes les tâches que ce qui peut être accompli dans la capacité de travail normale.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


Le coût total des heures supplémentaires pour une ressource sur toutes les tâches assignées.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


Le taux de rémunération des heures supplémentaires effectuées par une ressource.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Les unités utilisées par Microsoft Project pour afficher le taux des heures supplémentaires.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


Le montant des heures supplémentaires prévu pour être effectué par une ressource sur une tâche et facturé aux taux des heures supplémentaires des ressources concernées.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


L'unité d'affectation maximale pour une ressource à tout moment pour toutes les tâches auxquelles la ressource est affectée.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


Le pourcentage de travail accompli sur toutes les tâches.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


L'orthographe phonétique du nom de la ressource. À utiliser uniquement avec le japonais.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


Le montant total du travail non supplémentaire prévu à être effectué par la ressource.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


La dépense prévue restante qui sera engagée pour terminer le travail prévu restant.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


La dépense supplémentaire prévue restante pour une ressource.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


Le montant du temps supplémentaire prévu restant.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


Le taux de rémunération pour le travail régulier, non supplémentaire, effectué par une ressource.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Les unités utilisées par Microsoft Project pour afficher le taux standard.

### START {#START}
```
public static final Key<Date,Byte> START
```


La date à laquelle une ressource assignée est prévue pour commencer à travailler sur une tâche.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


L'écart de planification de la valeur acquise, jusqu'à la date d'état du projet. SV est la différence entre le coût budgété du travail effectué (BCWP) et le coût budgété du travail planifié (BCWS).

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


Le type d'une ressource.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


L'identifiant unique d'une ressource.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


Le compte NT associé à une ressource.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


Le montant total de temps prévu pour une ressource sur une tâche.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


Le type d'un groupe de travail auquel une ressource appartient.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


La différence entre le travail de référence d'une ressource et le travail actuellement prévu.

