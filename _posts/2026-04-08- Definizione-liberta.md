---
layout: post 
title: "Definizione libertà (bozza)" 
author: "Exim Gealbhonn" 
categories: journal 
tags: [Filosofia Politica]
---

Sia $I$ un insieme di individui.
Sia $A$ l'insieme degli atti, in particolare $a \in A$ indica un'azione che un individuo specifico fa interagendo attivamente con un certo sottoinsieme di individui.
Chiameremo potere  una tripla $(i, a, C)$, dove $i \in I$, $a \in A$ e $C \subseteq I$, che leggermo come  ''$i$ può fare $a$ su $C$''. Ad esempio se $a$ significa "andare a cena il 25 dicembre 2026 con ", la tripla significherà che $i$ ha il potere di andare a cena il 25 dicembre 2026 con le persone nell'insieme $C$. Dove per "potere" si intende potere effettivo, se vuole può farlo (indipendentemente dall'opinione dei membri in $C$). 
Chiaramente, non tutte le triple possono essere sensatamente considerati poteri, in quanto per alcuni sottoinsiemi $C$ il significato semantico di $a$ cozzerebbe. Nel caso dell'azione sopra considerata, avrebbe poco senso ad esempio considerare $(i,a, \{i\})$, in quanto signicherebbe che "$i$ può andare a cena in 25 dicembre 2026 con se stesso", che ha poco senso (se non volendo essere proprio laschi con il significato delle parole). 
Un altro esempio potrebbe essere il caso in cui $a$ = "camminare", in questo caso, essendo che l'atto non è un'azione che coinvolge altre persone, $(i,a,C)$ potrebbe essere un potere nell'unico caso in cui $C=\emptyset$, altrimenti non avrebbe senso. 
Chiamiamo $P$ l'insieme dei poteri, ossia di terne come quelle di cui sopra, tale che il sottoinsieme $C$ su cui agisce l'agente $i$ sia sensato.
In generale riterremo che se $(i, a, C) \in P$, allora $i \notin C$.
Si sottolinea che le azioni $a \in A$ devono essere abbastanza precise tale che un qualsiasi agente, se posto di fronte alla domanda se accetterebbe di essere sottoposto a questa azione da parte di un qualche altro agente, saprebbe sempre rispondere.

Chiaramente un individuo vorrà poter fare determinate cose e vorrà che gli altri non facciano determinate cose verso se stesso. Cerchiamo di modellizzare queste idee. 
Intanto, definiamo per ogni $j \in I$, $P_j:=\{(i,a, C) \in P | i=j\}$, ossia l'insieme di tutti i possibili poteri a cui potrebbe accedere $j$.
Ad ogni agente $i\in I$, sarà associata una relazione di preordine $\leq^p_i$ su $\wp(P_i)$. Quiesta relazione di preordine (l'apice 'p' sta ad indicare che è la relazione sui poteri) tiene traccia delle preferenze sui set di poteri che l'agente stesso preferisce. Si tenga conto del fatto che non si sta imponendo che questa relazione abbia proprietà particolari, per cui di per sé un agente può ad esempio scegliere di perdere dei poteri (per cui $P_i$ non è necessariamente il massimo).

Ci resta da costruire l'oggetto che invece modellizza l'avversione che ha un agente rispetto a determinate azioni che lo coinvolgono. 
Definiamo per ogni $j \in I$, $V_j=\{(i,a,C) \in P | j \in C\}$, ossia l'insieme di tutti i possibili poteri che può subire $j$.
Ad ogni agente $i \in I$ sarà dunque associata una relazione di preordine $\leq^a_i$ su $\wp(V_i)$. Questa relazione (l'apice 'a' sta ad indicare che è la relazione delle azioni avverse) tiene traccia delle preferenze sui set di azioni che l'agente avversa. 

Per completare la nostra modellizzazione degli individui ci resta solo di capire come rappresentare le preferenze individuali sui vari assetti sociali. A tal fine indichiamo che $S$ l'insieme di tutti i possibili assetti sociali, e associeremo ad ogni $i \in I$ una relazione di preordine $\leq ^s_i$ su $S$, che descrive appunto la preferenza dell'agente $i$ in merito alle possibili modalità di organizzazione sociale.

La terna $(\leq^p_i, \leq^a_i, \leq^s_i)$ descrive nel nostro modello completamente l'individuo $i$. 

L'idea centrale del modello è che un  assetto sociale $s\in S$ è primariamente caratterizzato dal fatto che realizza determinati poteri, indipendentemente poi che vengano o meno sfruttati. In un particolare assetto sociale io potrò fare qualcosa, mentre in un altro non ne avrò più potere. Questa idea ci permette di definire la funzione $r: S \rightarrow \wp(P)$, che associa ad ogni assetto sociale i poteri che esso realizza. Questo è l'oggetto principale del nostro modello.
Infine definiamo $P_i^s := \{x \in P_i| x \in r(s)\}$. 
Definiamo anche $V_i^s:=\{x \in V_i | x \in r(s)\}$.

A latere, si tiene a sottolineare che includiamo nella trattazione anche gli atti che non riguardano altri individui (come ad esempio $a$= "camminare") in quanto un assetto sociale può modificare il potere di un individuo indipentemente che l'azione coinvolga terzi. Si pensi ad esempio ad una società che investe in ricerca medica e ha un servizio sanitario capillare, rispetto ad una che non lo fa, se $i$ ad esempio non ha le gambe, nella prima società $i$ può camminare (in quanto può accedere a delle protesi), mentre nella seconda no.

Ora indichiamo con $s_0$ l'assetto sociale attuale. Diamo le seguenti definizioni.

**Definizione** Diciamo che un agente $i$ ha *una possibile pretesa trasformativa* se esiste $s \in S$ tale che $P_i^{s_0} \leq^p_i P_i^s$.

**Definizione** Diciamo che un agente $i$ ha *una pretesa trasformativa* se esiste $s \in S$ tale che $P_i^{s_0} \leq^p_i P_i^s$, e $s_0 <_i^s s$.

**Definizione** Diciamo che un agente $i$ ha *una possibile pretesa trasformativa non coattiva* se esiste $s \in S$ tale che $P_i^{s_0} \leq^p_i P_i^s$, ed inoltre per ogni $j \in I \setminus \{i\}$ si ha che $V_j^{s_0}\leq^a_j V_j^s$.

**Definizione** Diciamo che un agente $i$ ha *una pretesa trasformativa non coattiva* se esiste $s \in S$ tale che $P_i^{s_0} \leq^p_i P_i^s$, per ogni $j \in I \setminus \{i\}$ si ha che $V_j^{s_0}\leq^a_j V_j^s$ ed infine $s_0 <_i^s s$.

Uno stirneriano endorserà qualsiasi pretesa trasformativa, coattiva o meno che sia, altre scuole invece endorseranno solo quelle non coattive. 
La distinzione fra possibile ed effettiva pretesa trasformativa serve per tener conto del fatto che un agente non considera solo del proprio potere quando decide se vuole cambiare sistema sociale, ma farà altre considerazioni, che possono riguardare ad esempio le possibili interazioni avverse che potrebbe subire nel nuovo assetto sociale, come anche considerazioni in merito alla perdita di potere di altri agenti. In particolare l'introduzione della relazione d'ordine sugli assetti sociali ci permette di non imporre che gli agenti siano egocentrici.

**Definizione** Diremo che un agente $i$ è libero in $s\in S$ sse nell'assetto sociale $s$ attuale non ha pretese trasformative non coattive.

**Definizione** Diremo che l'assetto sociale $s\in S$ *produce una società libera* se in $s$, per ogni $i \in I$, $i$ è libero.

L'idea è quella che quando c'è una pretesa trasformativa non coattiva, è presente un conflitto fra gli agenti, e che questo conflitto debba risolversi con un cambiamento di assetto sociale a favore di chi ha la pretesa trasformativa non coattiva. 
Possiamo distinguere due tipi di conflitto.

**Definizione** Diremo che una pretesa trasformativa non coattiva è *generata da un conflitto nell'amministrazione delle cose* se, chiamato $s$ un assetto sociale che realizza la definizione di pretesa trasformativa non coattiva e $s_0$ l'assetto sociale attuale, nel momento in cui si cambiasse l'assetto sociale in $s$ un altro agente avrebbe una pretesa trasformativa non coattiva che sarabbe realizzata da $s_0$.

**Definizione** Se una pretesa trasformativa non coattiva non è generata da un conflitto nell'amministrazione delle cose, allora diremo che è una pretesa *generata dal dominio delle persone*.




