# act1

```
SceneSetup.act1();
```

(...300)

n: IAR ACEASTA ESTE ANXIETATEA ACESTUI OM

n: _TU_ EȘTI ANXIETATEA

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Hey hey! Iar am ajuns aici?

`hong({eyes:"0_neutral"})`

n: SCOUPUL TĂU E SĂ-ȚI PROTEJEZI OMUL DE *PERICOL*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FAPT, RELUAREA JOCULUI ĂSTUIA ÎL PUNE *ÎN PERICOL* FIX ACUM

n: REPEDE, AVERTIZEAZĂ-L!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Omule! Ascultă-mă te rog, suntem în pericol! Jucătorul...

[...o să ne tortureze iar!](#act1_replay_torture)

[...n-o să găsească un alt final!](#act1_replay_alternate)

[...o să intre în disonanță ludonarativă!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: O să ne facă să plângem în pat în poziția fetus!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: O să ne facă să spargem telefonul pt că ne-a dat un atac de panică!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: O să ne convingă să *NU* o pocnim pe gazdă!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: O să ne convingă să pocnim gazda asta super drăguță anti-erou!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Măcar tura asta e posibil să nu mai sărim de pe acope----
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: O SĂ NE FACĂ SĂ SĂRIM DE PE ACOPERIȘ.
{{/if}}

`bb({body:"fear"});`

b: O SĂ PĂȚIM TOATE LUCRURILE ASTEA ORIBILE ȘI-APOI O SĂ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Da fie, povestea în *întregul ei* e la fel, dar fiecare capitol are două posibile sfârșituri, plus toate variantele de dialo----

`bb({body:"fear"});`

b: Jucătorul o să fie dezamăgit, o să închidă tabul, o să șteargă softul, și apoi o să--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Lasciv ce..?

`bb({eyes:"normal"});`

b: Arcul poveștii era despre cum poți de fapt *SĂ ALEGI* să colaborezi în mod sănătos cu propria ta frică,

`bb({eyes:"normal_right"});`

b: dar când joci din nou jocul primești aceeași poveste, ceea ce înseamnă că *ALEGERILE* tale nu contează,

`bb({eyes:"narrow_eyebrow"});`

b: demonstrând astfel o contradicție între mesajul jocului și mecanica jocului,

`bb({eyes:"fear"});`

b: și dezvăluind conținutul acestui univers narativ,

`bb({body:"fear"});`

b: în care noi o să--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MURIIIIIIIIIIIIIIIIM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Okay hai să revenim în pielea personajului..

```
Game.clearText();
```

n4: (FOLOSEȘTE ANXIETATEA _TA_ BLA BLA BLA DE CE ANUME ȚI-ESTE _ȚIE_ CEL MAI FRICĂ BLA BLA ȘTII DEJA)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Super, s-a-ntors lupoaica. Exceleeeeeeeent.

`hong({eyes:"0_neutral"})`

n: SCOPUL TĂU E SĂ-ȚI PROTEJEZI OMUL DE *PERICOL*.

`bb({eyes:"look", mouth:"small_lock"})`

n: SANDWICH UL ĂLA ÎȚI PUNE OMUL ÎN *PERICOL* FIX ACUMA

n: REPEDE, AVERTIZEAZĂ-L!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Om! Omule, suntem în pericol! Iar pericolul este...

`bb({body:"squeeze"})`

n4: (SCOATE-ȚI ANXIETATEA _TA_ LA LUMINA, ALEGE OPȚIUNEA CARE E CEA MAI APROAPE DE CE ȚI-E _ȚIE_ FRICĂ)

(#act1_normal_choice)

# act1_normal_choice

[Mâncăm prânzul singuri! Iar!](#act1a_alone) `bb({body:"squeeze_talk"})`

[În timpul mesei nu suntem productivi!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Pâinea asta albă e nesănătoasă!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Stiai că singurătatea îți crește șansele să mori prematur la fel de mult cât ți-ar crește dacă ai fuma 15 țigări pe zi?

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Um, îți mulțumesc că dai surse dar--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Ceea ce înseamnă că dacă nu ne vedem cu cineva *chiar acum* atunci o să-

`bb({body:"panic"})`

b: MURIIIIIIIIIIIIIIIIM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: AI FOLOSIT *FRICA DE A NU FI IUBIT*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Scoate-ți laptopul și pune-te să faci ceva fix acuma!

`hong({eyes:"0_annoyed"})`

h: Parcă n-aș risca să-mi intre firimituri în tasta----

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Dacă nu contribuim ceva la corpul societății atunci suntem un parazit social!

b: Corpul-societal va merge la doctorul-societal că să-i dea tratament pentru paraziții-societali și-atunci noi o să--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MURIIIIIIIIIIIIIIIIM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: AI FOLOSIT *FRICA DE A FI O PERSOANĂ REA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Dar au fost sau nu replicate studiile as--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Grâul procesat o să ne ridice nivelul glicemiei în sânge și-o să trebuiască să ne amputeze membrele și-o să-

`bb({body:"panic"})`

b: MURIIIIIIIIIIIIIIIIM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: AI FOLOSIT *FRICA DE A FI RĂNIT*

(#act1b)

# act1b

n: E SUPER EFICIENT

`bb({mouth:"smile", eyes:"smile"});`

b: Vezi, omule? Sunt lupul tău loial de pază!

`bb({body:"pride_talk"});`

b: Ai încredere în ce simți! Sentimentele tale sunt mereu valide!

`bb({body:"pride"});`

n: ADU-I NIVELUL DE ENERGIE LA ZERO

n: PROTEJEAZĂ-I INTEGRITATEA FIZICĂ + SOCIALĂ + EMOȚIONALĂ, CU:

n: FRICA DE *A FI RĂNIT* #harm#

n: FRICA DE *A NU FI IUBIT* #alone#

n: ȘI FRICA DE *A FI O PERSOANĂ REA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (SFAT: ALEGE OPȚIUNILE CARE ÎȚI ATING ȚIE FRICILE TALE CELE MAI ADÂNCI!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: cred că-i timpul să-mi verific telefonul.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEJEAZĂ-ȚI OMUL

n: DE LUME. DE ALȚI OAMENI. DE EI ÎNȘIȘI.

n: SUCCES

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: RUNDA UNU: *LUPTAȚI!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Facebook zice că-i o petrecere weekendul ăsta care vine.

`bb({eyes:"uncertain"});`

b: Dubiosul acela nu dă petreceri în *fiecare* weekend?

`bb({eyes:"uncertain_right"});`

b: Ce gol interior existențial încearcă să umple? Tre să aibă mari probleme!

`hong({eyes:"surprise"});`

h: Hm, și pare că m-au invitat..?

`bb({eyes:"fear", mouth:"normal"});`

b: Hm!

[Zi da, altfel murim de singurătate!](#act1c_loner)

[Zi nu, e plin de droguri periculoase!](#act1c_drugs)

[Ignoră-l, stricăm oricum vibe-ul la orice petrecere.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Cincisprezece țigări pe zi, om! Cincisprezece!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Nu va veni nimeni la înmormântarea noastră, cenușa ne-o aruncă în ocean, apoi ne mănâncă o balenă,
{{/if}}

{{if !_.fifteencigs}}
b: și devenim CACA DE BALENĂ!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Așa că da, ar trebui să mergem la petrecerea aia!
{{/if}}

{{if _.parasite}}
b: Dar să iei laptopul că să lucrăm ceva, să nu fim parazit social.
{{/if}}

{{if _.whitebread}}
b: Atâta vreme cât pâinea nu e albă.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DOAMNE. Fie, dacă asta te face să taci.

h: O să zic da.

{{if _.whalepoop}}
b: Caca de balenă, omule! Caca de balenă!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: sau și mai rău.. PÂINE ALBĂ!
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Vom face supradoză de metanfetamină și pâine albă încât n-o să ne încapă cadavrul gras pe poarta crematoriului!
{{/if}}

{{if !_.whitebread}}
b: Vom face supradoză de așa multe droguri încât se vor întreba la pompe funebre  cum de e corpul *deja* îmbălsămat!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Oricum n-avem timp de petrecere, trebuie să lucrăm, altfel suntem un parazit social oribil!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DOAMNE. Fie, dacă asta te face să taci.

h: O să zic nu.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tot ce facem e să plângem într-un colț despre cum singurătatea e la fel de mortală ca 15 țigări pe zi.
{{/if}}

{{if _.parasite}}
b: Tot ce facem la petreceri e să ne gândim că ar trebui să facem ceva productiv în timpul ăsta.
{{/if}}

{{if _.whitebread}}
b: Tot ce facem e să ne gândim că alegerile culinare nesănătoase o să ne omoare până la urmă.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: oare de ce.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Deci dacă mergem îl supărăm, dar îl supărăm și dacă nu mergem și îi refuzăm invitația!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: FACEM OAMENII SĂ SE SIMTĂ RĂU, AR TREBUI SĂ NE SIMȚIM ȘI NOI RĂU

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Fie, dacă asta te face să taci.

h: Am să-i ignor invitația.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: În fine. Facebook e prea intes. Am nevoie de ceva mai calm, ceva ce nu-mi provoacă atâta anxietate.

`hong({eyes:"neutral"});`

h: Pe Twitter ce-o mai fi nou?

`bb({eyes:"look"});`

[Oh nu, ce știre absolut dezgustătoare!](#act1d_news)

[Oh nu, oare tweet-ul asta e de fapt despre *noi*?](#act1d_subtweet)

[Ei ia uite, un gif animat c-o pisică care bea lapte!](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Oh Doamne, pare că lumea o ia complet razna, nu?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Pare că totul e din ce în ce mai nasol și noi ne prăbușim o dată cu lumea și nu putem face absolut nimic în legătură cu asta.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Hai să dăm retweet știrii ăsteia!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Okay îi dau retweet dar te rog, gata, chill.

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Rahat, hai și pe Snapchat dacă tot.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: E un subtweet! E un subtweet de fapt, un subtweet insidios!

`hong({eyes:"annoyed"});`

h: Ba probabil că nu e..

`bb({eyes:"narrow", mouth:"small"});`

b: dar dacă vorbesc cu toții pe la spatele nostru

h: Nu-i adevăr--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ÎN FAȚA SPATELUI NOSTRU

`hong({eyes:"sad", mouth:"sad"});`

h: Nu cre--

`bb({eyes:"narrow", mouth:"small"});`

b: dar *dacă totuși*

h: T--

`bb({eyes:"narrow_eyebrow"});`

b: *dacă totuși*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Bu-buuuun, o să încerc Snapchat..

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: He-he ce drăguț, i-am dat retweet, cred că--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: PISICILE NU POT DIGERA LAPTELE, ORIBIL CĂ NE UITĂM LA AȘA CEVA ȘI ÎNCURAJĂM ABUZUL ANIMALELOR

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Bu-buuuun, o să încerc Snapchat...

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Ia uite, poze de la petrecerea de aseară. Deci așa arată petrecerile astea săptămânale.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, mult prea aglomerat pentru anxietatea mea..

h: Poate că n-ar fi trebuit totuși să accept invitația?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Schimbă răspunsul? Ca un prostovan?](#act1e_yes_dontchange)

[Schimbă răspunsul! E prea aglomerat!](#act1e_yes_changetono)

{{if _.subtweet}}
[Da, absolut era un subtweet.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Rahat, am dat retweet fără să verificăm sursele.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Știi că ai o postură foarte proastă?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Am răspuns deja da și contau pe noi că venim iar acum le trădăm încrederea, vrei să mori singur??!

{{if _.fifteencigs}}
b: CINCISPREZECE. ȚIGĂRI.
{{/if}}

{{if _.whalepoop}}
b: CACA. DE BALENĂ.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Taci, taci, îmi mențin răspunsul, rămâne da!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Cum se cheama aglomeratiile in care mori calcat pe cap? 

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: În 2003 a fost un incendiu într-un club in Rhode Island și de panică oamenii au blocat ieșirile și 100 de oameni au murit.-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VREI SĂ NI SE ÎNTÂMPLE ASTA ȘI NOUĂ-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: ZI NU ZI NU ZI NU ZI NU ZI NU ZI NU ZI NU ZI NU ZI NU ZI NU-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Gata, îmi schimb răspunsul, refuz invitația. Doamne ferește.

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... arată super distractiv.

h: Poate că n-ar fi trebuit să refuz invitația?

`bb({mouth:"normal", eyes:"normal"});`

[Schimbă răspunsul? Ca un prostovan?!](#act1e_no_dontchange)

[Schimbă răspunsul! Vei muri singur!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Yeah they were totally subtweeting us.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Rahat, am dat retweet fără să verificăm sursele.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Știi că ai o postură foarte proastă?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Toată lumea conta pe noi!!

b: ...să îi lăsăm în pace să se bucure de petrecere fără să aibă grija unui dubios dezgustător și oribil {{if _.whitebread}}mâncător-de-pâine-albă{{/if}} ca--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Okay gata taci taci, rămâne nu!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Singurătatea cronică ne crește nivelul de cortizol și riscul de boli cardiovasculare și de accident vascular cerebral!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: CINCISPREZECE. ȚIGĂRI.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Okay taci taci îmi schimb răspunsul, îi spun da!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Toate tweeturile noastre problematice din trecut au revenit în feed!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: O să fim scoși în evidență, o să fim cancelled și-apoi o să fim trași legați de cal pe autostrada informației!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: De ce te comporți așa?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Distribuim informații false! Distrugem încrederea oamenilor în presa liberă!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Noi suntem motivul pentru care se înalță fascismul din ruinele democrației!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: De ce te comporți așa?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vrei să ți se facă coloana covrig?! Nu mai sta așa cocârjat în fața ecranului!

```
bb({body:"meta"});
```

b: Și tu.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: De ce te comporți așa?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... arată destul de fain.

h: Poate că nu ar fi trebuit să ignor invitația?

`bb({mouth:"normal", eyes:"normal"});`

[Continuă să ignori, spargem cheful tuturor.](#act1e_ignore_continue)

[De fapt, zi da.](#act1e_ignore_changetoyes)

[De fapt, zi nu.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: E destul de nepoliticos să continui să-i ignori, nu?

`bb({eyes:"normal_right"});`

b: Lumea ne ignoră *pe noi* tot timpul așa că

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: să zicem că suntem chit.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Mă lași în pace să mă simt și eu.. bine?

b: Păi singurătatea ne poate *literal* omorî.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: E prea aglomerat. Mulțimile sunt periculoase..

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: În fine. Am primit notificare pe Tinder.

`bb({eyes:"uncertain"})`

b: Aplicația de babardeală?

`hong({eyes:"annoyed"})`

h: Nu e aplicație de babardeală.. e o platformă pentru cunoscut alți oa--

`bb({eyes:"narrow"})`

b: E aplicație de babardeală.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Suntem compatibili! Arată drăguț!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Să nu-mi strici te rog ast--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERICOL PERICOL PERICOL PERICOL PERICOL PERICOL

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Suntem *folosiți* de alți oameni.](#act1f_used_by_others)

[Ne *folosim* de alți oameni.](#act1f_using_others)

[PERSOANA ASTA ESTE UN CRIMINAL IN SERIE](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Întâlnirile astea aleatorii mă ajută să umplu golul pe care îl simt aici,

b: dar nu pot niciodată umple golul ...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: de *aici*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ideea e că VOM MURI SINGURI

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Ți se pare că organele genitale ale altor oameni sunt niște Pokemoni care așteaptă să-i colectăm noi?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon theme song)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ I wanna be, the ^slut^ti-est-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Like no one ever was-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Thighs n' ^ass^, voluptuous breast-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ with sweaty ^dick^ and balls!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PERVY-MON! GOTTA CA-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ideea e că suntem un dubios manipulativ.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: O să te-nchida într-o pivniță și-o să te forțeze să mănânci numai pâine albă că să te îngrașe să îți poarte pielea că pe-un costum!!
{{/if}}

{{if _.parasite}}
b: O să te măcelăreasca c-un ceas Pomodoro în timp ce țipă TREBUIA SĂ FII MAI PRODUCTIV PARAZITULE
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: O să - ți rupă carnea în bucăți confetti, carcasa ți -o folosesc drept strecurătoare și sângele ți -l pun cocktailuri!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Cum ți se pare ca text pt o invitație la petrecere?
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: așa m-am săturat de jocul ăsta.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"ne omoară singurătatea"... {{/if}}
{{if _.parasite}}"suntem paraziți sociali"... {{/if}}
{{if _.whitebread}}"nu mânca asta, o să ne omoare"... {{/if}}
{{if _.subtweet}}"ne vorbesc pe la spate"... {{/if}}
{{if _.badnews}}"lumea arde"... {{/if}}
{{if _.hookuphole}}"murim singuri"... {{/if}}
{{if _.serialkiller}}"criminal în serie"... {{/if}}
{{if _.catmilk}}"pisicile nu pot digere laptele"... {{/if}}
{{if _.pokemon}}"o melodie de parodie de ^căcat^... {{/if}}

h: nu vreau decât să îmi trăiesc viața.

h: vreau doar să nu mai simt atâta.. durere.

`bb({eyes:"look_sad"});`

b: Hey... omule...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: O să fie bine.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: În calitate de lupoaică de gardă, o să fac tot ce pot să te apăr și să te țin în siguranță..

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Promit.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ultima aplicație. Instagram. Să vedem.

`hong({eyes:"sad"});`

h: Și mai multe poze de la petrecere..

`hong({mouth:"sad"});`

h: Toată lumea pare așa de fericită. Nici o grijă. Nici urmă de anxietate.

`hong({mouth:"anger"});`

h: De ce nu pot fi ca ei? De ce nu pot fi și eu un om *normal?*

`bb({eyes:"normal_right"});`

b: Apropo de petreceri, uite decizia mea FINALĂ cu privire la invitația pt weekendul ăsta:

`bb({eyes:"normal"});`

[Ar trebui să mergem.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Nu ar trebui să mergem.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Nu ar--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: Bag

`hong({body:"2_you"});`

h: *^PULA^*.

(...500)

b: c

(...1500)

`bb({eyes:"wat_2"});`

b: ce..ce?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Am să răspund DA invitației ăleia,

{{if _.act1g=="go"}}
h: NU pentru că așa vrei tu, ci pentru că așa vreau *EU.*
{{/if}}

{{if _.act1g=="dont"}}
h: Exact pentru că tu vrei să NU merg.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: NU mă controlezi tu pe mine.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Acuma scuză-mă te rog cât mănânc și eu sandwichul ăsta de ^căcat^ în liniște..

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH O SĂ MURIM](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TOATĂ LUMEA NE URĂȘTE](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SUNTEM ABSOLUT ORIBILI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH O SĂ MURIM AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TOATĂ LUMEA NE URĂȘTE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SUNTEM ABSOLUT ORIBILI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: FELICITĂRI

(...500)

n: AI PROTEJAT CU SUCCES INTEGRITATEA FIZICĂ, SOCIALĂ ȘI EMOȚIONALĂ A OMULUI TĂU

n: UITE NUMAI CE RECUNOSCĂTORI SUNT!

(...500)

n: ACUMA CĂ ENERGIA LOR E LA ZERO, LE POȚI CONTROLA DIRECT ACȚIUNILE

`bb({mouth:"smile", eyes:"normal"});`

n: ALEGE-ȚI MUTAREA FINALĂ

`bb({mouth:"small_lock", eyes:"fear"});`

n: *TERMINĂ-I*

[{LUPTĂ: pedepsește-ți telefonul, e vina lui!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGI: începe să plângi în poziția fetus}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Telefonul tău îți provoca un atac de panică!

`bb({eyes:"anger"})`

b: Zuckerberg și gașca lui îți scurtcircuitează creierul pentru bani!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Pedepsește-ți telefonul! Distruge-l! Omoară-l!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOARĂ-L! OMOA--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Lumea a plină de pericole!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fă ce face armadillo-ul! Ghemuiește-te într-o bilă auto-protectoare!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: GHEMUIEȘTE-TE ȘI PLÂNGI GHEMUIEȘTE-TE ȘI PLÂNGI GHEMUIEȘTE-TE ȘI PLÂNGI GHEMUIEȘTE-TE ȘI PLÂNGI GHEMU-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`