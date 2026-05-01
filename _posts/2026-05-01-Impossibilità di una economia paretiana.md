---
layout: post 
title: "Impossibilità di una economia paretiana" 
author: "Exim Gealbhonn" 
categories: journal 
tags: [Filosofia Politica]
---

# Impossibilità di una economia di scambio paretiana senza ipotesi di egocentrismo

Come è noto dalla microeconomia, sotto certe ipotesi sulle preferenze degli agenti in merito alle distribuzioni sociali di beni (razionalità, egocentrismo, continuità), è sempre possibile trovare almeno una distribuzione che sia ottima secondo Pareto e al contempo sia preferita alla distribuzione iniziale dei beni, e tale che gli agenti non hanno più interesse a scambiare. 
Un quesito che ci si può porre è se è possibile avere un risultato simile indebolendo l'ipotesi sulle preferenze degli agenti. In questo articolo vedremo come il risultato decade se si elimina l'ipotesi di egocentrismo (e ci sono almeno 4 agenti).


## Modello di Arrow-Debreu e notazione
Ci concentreremo sul caso di una economia senza produzione. In particolare ricostruiremo il classico modello di Arrow-Debreu, ma non imporremo la condizione di egocentrismo

Il problema è quello di distribuire un paniere di $m \in \mathbb{N}$ beni limitati fra $l \in \mathbb{N}$ agenti. La quantità di beni disponibili  alla società è data dal vettore $\Omega=(x_1^{max},... x_m^{max})$, dove

$$ x_i^{max} \in \mathbb{R}_+$$  

rappresenta la quantità del bene $i$-esimo disponibile. 
Il problema è capire come distribuire i beni del vettore $\Omega$ fra i vari agenti, ossia come associare ad ogni agente $i$ un paniere di beni $p^i \in \mathbb{R_+^m}$, che conterrà appunto l'informazione su quali beni possederà l'agente $i$ e in che quantità.
Una qualsiasi $l$-upla di panieri $\mathbf{p}=(p^1,..., p^l)$ sarà detta una allocazione. Visto che le quantità di beni sono limitate, non tutte le allocazioni di beni sono ammissibili, per cui diremo che una allocazione $\mathbf{p}$ è realizzabile se è una allocazione che rispetta la seguente proprietà

$$ \sum_{i=1}^l p^i=\Omega. $$

In particolare si noti che una allocazione realizzabile è una in cui tutti i beni vengono distribuiti (ossia nessun bene resta senza proprietario). Si noti inoltre che questa definizione di allocazione realizzabile implica implicitamente che i beni sono infinitamente divisibili (ci si può chiedere della sensatezza di avere come allocazione realizzabile una in cui possiedo una quantità di pane inferiore alle costante di Plank, ma questo passa il convento).

Chiamiamo $S$ l'insieme delle allocazioni realizzabili.

Per capire come selezionare l'allocazione ""migliore"" fra quelle presenti in $S$ possiamo chiederci quale sia la preferenza dei vari agenti in merito a queste allocazioni in $S$, e poi a partire da esse cercare di dare una serie di condizioni che desideriamo abbia la nostra allocazione ottimale. Auspicabilmente saremmo molto contenti se dopo aver posto questi desiderata, trovassimo che una sola allocazione ottimale li rispetta. 
Per fare ciò quindi associamo ad ogni agente $i \in \lbrace 1,..., l\ rbrace$ una relazione transitiva e completa, ossia un preordine completo, su $S$. Indicheremo tale relazione con la notazione $\leq^i$, la cui interpretazione è quella che se vale $\mathbf{p}_1 \leq^i \mathbf{p}_2$, allora l'agente $i$ preferisce l'allocazione $\mathbf{p}_2$ a $\mathbf{p}_1$ (oppure è indifferente fra le due allocazioni). In particolare la condizione di transitività e completezza sono quelle che in letteratura economica sono quelle che caratterizzano la nozione di "razionalità". 
Noi oltre alla razionalità imporremo che questi preordini siano continui, ossia che, senza entrare eccessivamente nei dettagli,  possiamo rappresentare i nostri preordini come funzioni d'utilità continue (con topologia prodotto e poi topologia sottospazio su S).
Questa ipotesi è rilevante in quanto (come ben vedremo dopo) nel caso in cui le possibili opzioni fra cui scegliere sono infinite (come in questo caso), allora non è garantito che esista un ottimo di Pareto, per cui tutta la presente discussione sarebbe un po' vuota, ma con l'ipotesi di continuità l'esistenza di almeno uno è garantita. Si noti comunque che se facciamo decadere che i beni sono infinitamente divisibili, avremo $S$  finito, e l'ipotesi di continuità in questo caso è sempre soddisfatta da qualsiasi preordine completo.

Adesso diamo una definizione della nozione di egocentrismo.

**Definizione** Diremo che un agente $i$ è egocentrico se, di fronte alla scelta fra due allocazione $\mathbf{p}_2$ a $\mathbf{p}_1$, nel caso in cui $p^i_1 = p^i_2$, allora $\mathbf{p}_2 \sim \mathbf{p}_1$ (ossia vale $\mathbf{p}_1 \leq^i \mathbf{p}_2$ e $\mathbf{p}_2 \leq^i \mathbf{p}_1$). 
Diremo che sussiste l'ipotesi di egocentrismo se ogni agente $i$ è egocentrico.

Detto altrimenti, un agente egocentrico è interessato solo al proprio paniere, ed è totalmente indifferente a quello che otterranno gli altri dalla distribuzione. Si noti che sotto questa ipotesi gli agenti non possono essere né altruisti (magari preferendo allocazioni in cui gli altri stanno meglio, o magari preferendo distribuzioni più eque in qualche senso), né egoisti (non si può preferire una allocazione ad un'altra perché banalmente ho piacere che qualcun altro stia peggio). 
Noi non imporremo questa condizione, e questo ci porterà al risultato di impossibilità.

Chiameremo $\Sigma$ l'insieme di tutti i preordini completi e continui su $S$.

Fatte queste premesse iniziamo a dare alcune definizioni utili per definire i nostri desiderata. 
Partiamo con l'ottimalità di Pareto. 

**Definizione** Diremo che una allocazione realizzabile $\mathbf{a} \in S$ è un ottimo (stretto) di Pareto sse non esiste alcun $\mathbf{b} \in S$ tale per cui vale ($\mathbf{b} \ge^i \mathbf{a}$ per ogni $i \in \lbrace1,..., l
brace$, ed esiste $j \in\lbrace1, ..., l
brace$ tale che $\mathbf{b} >^i \mathbf{a}$).

**Definizione** Diremo invece che una allocazione realizzabile $\mathbf{a} \in S$ è un ottimo (debole) di Pareto sse non esiste alcun $\mathbf{b} \in S$ tale per cui vale $\mathbf{b} >^i \mathbf{a}$ per ogni $i \in \lbrace1,..., l
brace$.

È immediato dimostrare che un ottimo stretto di Pareto è anche un ottimo debole di Pareto.

Un altro elemento molto importante del presente modello è quello che i beni in $\Omega$ sono in realtà già tutti distribuiti in partenza, ossia tutti i beni all'inizio del processo distribuitivo hanno già un proprietario, quindi in realtà il problema è quello di capire come "ottimizzare" (idealmente via scambi) questa allocazione originaria. 

**Definizione** Chiamiamo $\mathbf{o} \in S$ l'allocazione originaria. Diremo che una allocazione $\mathbf{a} \in S$ rispetta l'allocazione originaria se per ogni $i$ vale che  $\mathbf{a} \ge^i \mathbf{o}$.

Infine diamo una condizione di "ottimalità" nel senso di scambi.

**Definizione** Diremo che una allocazione $\mathbf{a} \in S$ è stabile per scambi se non esiste alcuna altra allocazione $\mathbf{b} \in S$ tale che $\mathbf{a}$ e $\mathbf{b}$ differiscono unicamente per i panieri di due agenti $i$ e $j$, e vale che $\mathbf{b}>^t\mathbf{a}$ per $t \in \lbracei,j
brace$.

L'interpretazione di questa definizione è che, se si realizza una allocazione che è stabile per scambi, nessuno ha più possibilità di scambiare.

Adesso imponiamo i nostri desiderata.

**Definizione** Diremo che una allocazione $\mathbf{a} \in S$ è selezionabile (strettamente o debolemente) se rispetta l'allocazione originaria, è un ottimo di Pareto (risp stretto o debole), e inoltre è una allocazione che è stabile per scambi.
[Sostanzialmente l'idea è che l'allocazione finale che si realizzerà sarà selezionata all'interno nell'insieme delle allocazioni selezionabili]

Infine diremo che esiste un equilibrio economico generale (stretto o debole) su un sottoinsieme $K \subseteq \Sigma^l$ se per ogni $k \in K$ l'insieme delle allocazioni selezionabili (strettamente o debolmente risp.) è non vuoto.

Diremo che esiste un equilibrio economico generale con dominio non ristretto se $K=\Sigma^l$.

Facciamo alcuni commenti su quanto detto. Usando questo linguaggio, se chiamiamo $K_e$ il sottoinsieme di $\Sigma^l$ in cui ogni $k \in K^*$ è composto solo da preferenze egocentriche, allora il classico risultato di Debreu può essere riscritto in questi termini:

**Teorema (Debreu)**  Per ogni $K \subseteq K^*$, esiste un equilibrio economico generale stretto su $K$.

Ora qualcunx potrebbe contestare l'utilizzo del termine "equilibrio economico generale" in questo contesto, in quanto questo linguaggio è solitamente associato ai teoremi dell'economia, e fa riferimento in particolare a quelle allocazioni selezionabili che sono ottenibili via ricerca degli zeri di una funzione eccesso di domanda. 
Chiaramente non è il nostro caso, nel contesto generale in cui ci stiamo ponendo (in cui accettiamo anche agenti non egocentrici) questo tipo di desiderata di "annullamento della funzione eccesso di domanda" sarebbe complicato da porre, infatti anche riuscissimo a riformulare l'ipotesi di agenti price-taker senza l'ipotesi di egocentrismo, comunque non è evidente quale sarebbe la strategia ottimale degli agenti (e quindi sarebbe complicato definire come costruire la funzione eccesso di domanda). Di contro, il nostro obiettivo è ancora più profondo, ossia quello di dimostrare che anche se riuscissimo a costruire una funzione eccesso di domanda, e questa ammettesse zeri, comunque non avremmo garantito che quelli zeri generino allocazioni selezionabili. In definitiva, non possiamo dire che l'incontro fra domanda e offerta produca allocazioni "efficienti". Il nostro obiettivo infatti è dimostrare il seguente teorema:

**Teorema (Impossibilità)** Non esiste un equilibrio economico generale debole con dominio non ristretto se $l \ge 4$

Quindi perché stiamo usando questa terminologia? Perché vogliamo porre l'accento sul fatto che ci stiamo interessando non solo al fatto che le allocazioni devono essere ottimi di Pareto e rispettare l'allocazione iniziale, ma anche che siano generabili via scambi (ossia che la dinamica di scambio non rompa l'efficienza paretiana).

Come piccola nota conclusiva di questa sezione, è rimasta sospesa la questione dell'unicità delle allocazioni selezionabili. Come è chiaro, dimostreremo che ci sono casi in cui non esistono allocazioni selezionabili, ma quando esistono sono uniche? La risposta in generale è no, anche sotto le ipotesi classiche dei teoremi dell'economia del benessere (dove si impongono altre ipotesi sugli agenti, sia sulle preferenze che sulla psicologia),e  guardando anche solo a quelle realizzabili via ricerca di zeri dell'eccesso di domanda, non c'è garanzia che le allocazioni "ottimali" siano uniche. Come reso evidente dall' ["Anything Goes Theorem"](https://en.wikipedia.org/wiki/Sonnenschein%E2%80%93Mantel%E2%80%93Debreu_theorem), le funzioni eccesso di domanda ottenibili sono davvero molto variegate, quasi arbitrarie e imprevedibili, quindi possiamo avere davvero un'ampia casistica di insiemi di allocazioni "ottimali". Questa arbitrarietà della funzione eccesso di domanda rende inoltre palesi che gli equilibri (nel processo di tâtonnement walrasiano) possono anche essere instabili e quindi non avere mai convergenza verso il sistema di prezzi ottimale (per chi volesse approfondire questo aspetto dinamico consiglio questo [articolo di Scarf](http://dido.econ.yale.edu/~hes/pub/instability.pdf)). Per avere l'unicità bisogna imporre condizioni strutturali molto stringenti (una delle condizioni sufficienti più note è quella per cui la funzione eccesso di domanda rispetti la proprietà di "Gross Substitutes"), ossia condizioni che riguardano il sistema economico in generale, e non solo il comportamento dei singoli agenti (o almeno, a me non sono noti risultati di questo tipo). Non approfondiremo oltre la questione dell'unicità.


## Dalla microeconomia alla teoria delle scelte sociali

Il nostro obiettivo adesso è quello di interpretare il modello di Arrow-Debreu che abbiamo abbozzato nel paragrafo precedente nel contesto della teoria delle scelte sociali, e da lì usare noti risultati di impossibilità per dimostrare il Teorema 2.
Iniziamo con la prima definizione

**Definizione** Sia $K \subseteq \Sigma^l$. Chiamere funzione di scelta sociale (in inglese "social choice function", da ora in SCF) con dominio $K$ una funzione $C:K\rightarrow S$

L'interpretazione di una SCF è banale, se il set di preferenze è $k \in K$, allora l'allocazione selezionata per essere quella definitiva sarà $C(k)$.

Ridiamo alcune definizione già viste nel paragrafo precedente, ma nel contesto delle SCF.

**Definizione** Data una allocazione iniziale $\mathbf{o}\in S$. Diciamo che una SCF $C$ con dominio $K$ rispetta l'allocazione iniziale se per ogni $k \in K$ vale che $C(k) \geq^i \mathbf{o}$ per ogni $i$.

**Definizione** Data una SCF $C$ con dominio $K$, diremo che rispetta il principio debole di Pareto se per ogni $k \in K$ e per ogni $\mathbf{a}, \mathbf{b} \in S$ tale che $\mathbf{a}<^i_k \mathbf{b}$ per ogni $i$, allora $C(k)\neq \mathbf{a}$.

**Definizione** Data una SCF $C$ con dominio $K$, diremo che è stabile per scambi se per ogni $k \in K$, $C(k)$ è un'allocazione che è stabile per scambi (in riferimento al set di preferenze $k$).
Detto altrimenti, se è possibile passare da $\mathbf{a}$ a $\mathbf{b}$ attraverso uno scambio fra 2 agenti, allora $C(k) \neq \mathbf{a}$.

Adesso dimostriamo la seguente proposizione.

**Proposizione** Sia $K \subseteq \Sigma^l$. Se esiste un equilibrio economico generale debole su $K$, allora esiste una SCF $C:K \rightarrow S$ che rispetta l'allocazione iniziale, il principio debole di Pareto ed è stabile per scambi.

**Dimostrazione** La dimostrazione è elementare. Preso un $k \in K$, basta associagli una qualche allocazione selezionabile scelta in qualche modo. In particolare chiamiamo $f:K \rightarrow P(S)$ la funzione che associa $k$ al suo corrispondente insieme di allocazioni selezionabili. Si noti che $\emptyset \notin f(K)$. Si noti in particolare che per l'assioma della scelta esiste una funzione di scelta $g: P(S) \setminus \lbrace\emptyset
brace \rightarrow S$. Per cui basta prendere $C=g \circ f$. Chiaramente per costruzione questa SCF rispetta le due proprietà. $\square$

Adesso diamo  altre due importanti definizioni

**Definizione** Data una SCF $C: K \rightarrow S$, diremo che un agente $i$  ha una libertà minimale rispetto a $C$ se esiste  $\lbrace\mathbf{a}_1, \mathbf{a}_2
brace \subset S$ (con i due elementi distinti) per cui valga la seguente proprietà:

$$ 
\mathbf{a}_s <^i_k \mathbf{a}_t \implies C(k)\neq \mathbf{a}_s
$$

per ogni $s, t \in \lbrace1,2
brace$, e $k \in K$.

 **Definizione** Data una SCF $C: K \rightarrow S$, diremo che $C$ rispetta l'ipotesi di liberalismo minimale se esistono almeno due individui distinti hanno una libertà minimale.

 Adesso dimostriamo il seguente importante teorema

 **Teorema (Sen per SCF)** Non esiste alcuna funzione di scelta su $\Sigma^l$ tale che rispetti il principio debole di Pareto e liberalismo minimale se ci sono almeno 2 individui.
 
 **Dimostrazione** Basta ricalcare la [dimostrazione del teorema di Sen](https://www.reforming.it/doc/1787/sen-impossibilityparetian.pdf), ma con qualche accortezza. Da questo momento in poi, quando dirò "preferiscono", intendo "preferiscono strettamente.". Inoltre si noti che le relazioni che costruiremo nel seguito è possibile renderle banalmente continue (se sommiamo, ""nel senso degli ordinali""", un preordine completo e continuo ad un preordine completo su un insieme finito di elementi, otteniamo ancora un preordine completo e continuo). 
 Siano gli individui $i$ e $j$ sono i due individui distinti che hanno una libertà, e la loro rispettive coppie su cui sono decisivi sono rispettivamente $\lbrace\mathbf{a}_1, \mathbf{a}_2
brace$ e $\lbrace\mathbf{b}_1, \mathbf{b}_2
brace$. 
 Nel caso in cui $\lbrace\mathbf{a}_1, \mathbf{a}_2
brace=\lbrace\mathbf{b}_1, \mathbf{b}_2
brace$, allora basta prendere un set di preferenze in cui tutti gli agenti preferiscono $\mathbf{a}_1$ e $\mathbf{a}_2$ a qualsiasi altra opzione, e tale che $i$  preferisca strettamente $\mathbf{a}_1$ ad $\mathbf{a}_2$, mentre $j$ preferisca $\mathbf{a}_2$ ad $\mathbf{a}_1$. Per principio di Pareto le uniche scelte possibili sono  $\mathbf{a}_1$ e $\mathbf{a}_2$, ma per per definizione di libertà minimale, nessuna delle due va bene. Per cui non esiste una funzione di scelta sociale.
 Nel caso in cui $\mathbf{a}_2 = \mathbf{b}_1$. Rinominiamo $\mathbf{a}= \mathbf{a}_1$, $\mathbf{c}= \mathbf{b}_1$ e  $\mathbf{b}= \mathbf{b}_2$. Adesso basta prendere un set di preferenze in cui tutti gli agenti preferiscono $\mathbf{a},\mathbf{b},\mathbf{c}$ a qualsiasi altra opzione, e tale che tutti preferiscano $\mathbf{a}$ a $\mathbf{b}$. Se ora l'agente $i$ preferisce $\mathbf{c}$ ad $\mathbf{a}$ e l'agente $j$ preferisce $\mathbf{b}$ a $\mathbf{c}$, si ottiene che non c'è alcuna scelta possibile per questa casistica. Infatti per Pareto le uniche opzioni possibili sono $\mathbf{a}$,$\mathbf{b}$,$\mathbf{c}$, ma per la definizione di libertà di $i$, $\mathbf{a}$ deve essere scartata, mentre per quella di $j$ ad essere scartato è $\mathbf{c}$, per cui l'unica opzione rimasta è $\mathbf{b}$, ma questa non va bene perché è dominata da $\mathbf{a}$, per cui $\mathbf{b}$ deve essere scartato per Pareto. Per cui non esiste una funzione di scelta sociale in questo caso.
 Il caso in cui sono tutti distinti è nello stesso spirito, ed è lasciato come esercizio al lettore. $\square$

Adesso preseguiamo cercando di dare una piccola versione alternativa di questo teorema. 
Diamo la seguente definizione

**Definizione** Chiameremo un insieme $\lbracei,j
brace$, con $i,j \in \lbrace1,...,l
brace$ (con $i \neq j$) una coalizione binaria. 

**Definizione** Data una SCF $C: K \rightarrow S$, diremo che una coalizione binaria $\lbracei,j
brace$  ha una libertà minimale rispetto a $C$ se esiste  $\lbrace\mathbf{a}_1, \mathbf{a}_2
brace \subset S$ (con i due elementi distinti) per cui valga la seguente proprietà:

$$ 
( \forall u \in \lbracei, j
brace\text{	}\mathbf{a}_s <^u_k \mathbf{a}_t) \implies C(k)\neq \mathbf{a}_s
$$

 per ogni $s, t \in \lbrace1,2
brace$, e $k \in K$.

 
 **Definizione** Data una SCF $C: K \rightarrow S$, diremo che $C$ rispetta l'ipotesi di liberalismo minimale per bicoalizioni se esistono almeno due coalizioni binarie con intersezione vuota che hanno una libertà minimale.

 **Teorema (Sen per coalizioni binarie)** Non esiste alcuna funzione di scelta sociale su $\Sigma^l$ tale che rispetti il principio debole di Pareto e liberalismo minimale per bicoalizioni se ci sono almeno 4 individui.

 **Dimostrazione** Essendo che l'intersezione fra le coalizioni è vuota, allora basta prendere i set di preferenze in cui gli individui della stessa coalizioni hanno lo stesso ordinamento, in particolare in questi set di preferenze le coalizioni si comportano come un individuo unico, per cui si può applicare Sen classico e ottenere la tesi.  $\square$

 ## Dimostrazione del teorema di impossibilità
Per risultati generali (sempre riconducibili a Debreu), noi sappiamo che date vale il seguente risultato

**Teorema (Debreu senza egocentrismo)** Per ogni $k \in \Sigma^l$, e per ogni dotazione iniziale $\mathbf{o} \in S$ , esiste una allocazione Pareto-efficiente stretta (e quindi anche debole) tale rispetti la dotazione iniziale $\mathbf{o}$.

Per cui, anche senza assumere egocentrismo, noi sappiamo che esiste una allocazione ottimale secondo Pareto preferita da tutti a quella iniziale. Ciò che dimostreremo è che non è detto che ne possiamo trovare una che è anche stabile per scambi. 

Rienunciamo il teorema.

 **Teorema 2. (Impossibilità)** Non esiste un equilibrio economico generale debole con dominio non ristretto se $l\ge 4$.
 
 **Dimostrazione**
Se per assurdo non valesse la tesi, per la Proposizione 1 varrebbe che esiste una SCF $C:\Sigma^l \rightarrow S$ che rispetta l'allocazione iniziale, rispetta il principio debole di Pareto, ed è stabile per scambi. Vogliamo dimostrare che questo è impossibile per il teorema di Sen per coalizioni binarie.
Per ipotesi sappiamo che esistono almeno quattro agenti distinti, chiamiamoli $A,B,C,D$. Vogliamo dimostrare che $\lbraceA,B
brace$ e $\lbraceC,D
brace$ sono due coalizioni binarie che hanno una libertà minimale. Infatti si noti che l'ipotesi che la SCF sia stabile per scambi impone che, date due allocazioni realizzabili$\mathbf{a}$ e $\mathbf{b}$ tali che differiscono unicamente per i panieri di $A$ e $B$, allora se entrambi preferisco $\mathbf{b}$ a $\mathbf{a}$, allora la società non può scegliere l'allocazione $\mathbf{a}$ (discorso simile vale per $C$ e $D$). Ma questa è esattamente la definizione di libertà minimale per coalizioni binarie. Per cui l'esistenza di $C$ implica l'esistenza di una SCF su $\Sigma^l$ che rispetta il principio di Pareto e liberalismo minimale per bicoalizioni. Assurdo per Sen. $\square$

## Ha senso non imporre l'egocentrismo?

Siamo riusciti a dimostrare che la dinamica di mercato, se gli agenti non sono egocentrici, non ci garantisce il raggiungimento di una allocazione che è efficiente secondo Pareto, anche se allocazioni efficienti esistono. La questone però adesso è chiedersi se effettivamente ha senso interessarsi di queste casistiche. Infatti se gli agenti fossero effettivamente egocentrici (quantomeno sul terreno economico), allora questo risultato avrebbe poco interesse teorico. Ora, chiaramente questa è una questione psicologica/antropologica/sociologica con ampia letteratura in merito, comunque la risposta pare essere di no, si pensi ai risultati di economia sperimentale in merito agli ultimatum game (o giochi simili). Probabilmente, però, la prova del nove è data dallo stuolo di imprenditori e liberali che si lamentano 24/7 sui media dell'invidia sociale dilagante; e se lo dicono loro, allora sarà vero che gli agenti non sono egocentrici :D

 
 

 

 
