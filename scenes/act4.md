# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (game auto-saved)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *of*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Așadar, care ^naiba^ a fost morala poveștii?

`hong({body:"one_up", eyes:"annoyed"})`

h: Ce am *învățat* măcar? Mă *comportam* într-un mod prostesc, "prietenii" mei mă *foloseau*, și eram aproape de a *muri*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Mda, ca să nu mai vorbim de bonul de la spital.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Mda, ca să nu mai vorbim de deteriorarea ficatului.](#act4a_liver)
{{/if}}

[Mda, ăla *era* scenariul cel mai prost.](#act4a_worst)

[Mda, am avut dreptate.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Corect. Nu cred ca asigurarea medicală îmi acoperă "imbecilitatea".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Și totuși... am supraviețuit!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Cu siguranță ne-am scurtat puțin din speranța de viață...

`bb({eyes:"surprise"});`

b: Dar măcar încă *avem* o speranță de viață! Am supraviețuit!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Și totuși...

h: Hm?

`bb({eyes:"surprise"});`

b: Am supraviețuit!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Însă... și tu ai avut dreptate.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Am *fost* lupul care a strigat lupul. Așadar când a fost *un adevărat* pericol, pe bună dreptate, nu m-ai crezut.

`bb({eyes:"surprise_r"});`

b: Și totuși, am supraviețuit!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: În ciuda a ce s-a întâmplat, încă suntem aici.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Pari destul de calm, având în vedere că tocmai am avut o experiență aproape de moarte.
{{/if}}

{{if !_.INJURED}}
h: Pari destul de calm, având în vedere că tocmai am avut o experiență *foarte* aproape de moarte.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Ei bine, asta face orice altceva mai puțin înfricoșător în comparație. Chiar m-a făcut să mă gândesc. 

`bb({eyes:"normal", mouth:"normal"});`

b: Dacă să mă cert cu tine este nașpa, pentru că nu te protejează...

h: Dar să mă cert *eu* cu tine este nașpa, pentru că te face să strigi mai tare...

`bb({eyes:"normal_r"})`

b: Poate atunci...

`bb({eyes:"normal"})`

h: Poate nu trebuie să ne certăm.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Nu sunt Lupul cel Rău. Dar nici câine de pază nu sunt. 

`bb({eyes:"sad_d"})`

b: Sunt un câine de adăpost schingiuit. 

`bb({eyes:"sad"})`

b: Am trecut prin chestii dure. Poate traumă sau neglijență. De aceea uneori mai exagerez și încep: 

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: HAM HAM HAM HAM HAM

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Dar nu *vreau* să fiu un câine fricos! Vreau să te protejez! Vreau să fiu un câine bun!

`bb({eyes:"sad", mouth:"normal"});`

b: Omule... vei ajuta cu îmblânzirea acestui lup? 

`hong({eyes:"sad"})`

h: Voi... Voi încerca. 

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: OK. O relație sănătoasă cu emoții. Relațiile au nevoie de comunicare. Deci, să comunicăm. 

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Următoarele cinci minute vor suna foarte siropoase, dar hai să ne prefacem până reușim. 

```
hong({body:"hands_2", mouth:"normal"});
```

h: Dragă lup interior... cum *te* simți? 

n2: FRICI FOLOSITE ÎN TOTAL:

n2: *A FI RĂNIT* {{_.attack_harm_total}}, *A NU FI IUBIT* {{_.attack_alone_total}}, *A FI O PERSOANĂ REA* {{_.attack_bad_total}}

n2: DESPRE CARE FRICĂ VREI SĂ VORBEȘTI ÎNTÂI? (POȚI TRECE PRIN CELELALTE MAI TÂRZIU)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Mi-e frică de a fi răniți.](#act4_harm)

[Mi-e frică de a fi singuri.](#act4_alone)

[Mi-e frică de a fi niște persoane rele.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Vreau să îți protejez nevoia de siguranță fizică,

`bb({eyes:"sad_d"})`

b: dar *toată lumea* pare atât de periculoasă. Atât de plină de tragedii și răutăți. 

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Nu știu, gata cu alegerea *mea* pentru următoarea replică. Ce ai *tu* de spus, omule? 
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Din nou, înapoi la tine, omule. Ce crezi? 
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Alte păreri, omule?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ai dreptate. Deci hai să fim mai protectivi cu noi înșine.](#act4_harm_skills)

[Hai să ne expunem la *mai multe* pericole.](#act4_harm_exposure)

[Mulțumesc.](#act4_thanks) `_.thanks_for = "siguranța fizică";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Dar... cum? Am eu colți și gheare, dar sunt doar o metaforă.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Am putea învăța să ne auto-apărăm? Să ne alăturăm unei comunități care se apără reciproc? Să ne îmbunătățim în general sănătatea și granițele personale?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Poate, dar...

[De unde începem măcar?](#act4_harm_skills_start)

[Dacă nu va funcționa?](#act4_harm_skills_work)

[Dacă vom exagera cu „siguranța”?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Sunt atâtea de făcut, atât de multe de reparat la noi. Cu ce *începem* măcar?

`hong({ body:"shrug", eyes:"surprise" })`

h: Începem chiar acum.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ha?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Practicăm o bună comunicare chiar acum. Care ne va ajuta să detectăm mai ușor pericolele, cu mai puține fals-pozitive,

`hong({ eyes:"surprise" });`

h: Iar *asta* ne va ajuta să ne protejeze de a fi răniți!

`hong({ eyes:"normal", mouth:"normal" });`

h: Așadar: acesta *este* un antrenament de auto-apărare.

`bb({ eyes:"normal_r" })`

b: Hm. Mă așteptam mai mult la asta:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Adevărat, nu este posibil să ne apărăm 100% de pericole...

`hong({ body:"one_up" });`

h: Dar până și o îmbunătățire de 1% merită ceva, corect?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Vezi paharul a nu fi 99% gol, dar 1% plin?

`bb({ eyes:"normal" });`

h: Care tot contează dacă ești blocat într-un deșert.

`bb({ eyes:"closed" });`

b: Ei bine. Până la fund, atunci. Well.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Adică, motivul principal pentru care mi-ai ignorat avertismentele a fost pentru ca *am* exagerat cu siguranța! 

`bb({ body:"normal", eyes:"normal" })`

h: Neh, ai dreptate. Am vrea să ne apărăm moderat. Totul să fie moderat.

`bb({ eyes:"suspect" })`

b: Scuză-mă, *TOTUL* să fie moderat?

`hong({ eyes:"annoyed" })`

h: *Un număr moderat de chestii* să fie moderat.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Mulțumesc pentru că te-ai străduit în mod repetat să-ți faci mărturiile consecvente.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *CE*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Adică, să spunem că unui câine îi e frică de tunet.

`hong({ body:"hands_1" });`

h: Un truc pe care dresorii îl folosesc este să redea o înregistrare a tunetului la volum mic, apoi îi oferă câinelui o recompensă pentru că a rămas calm.

`hong({ body:"hands_2" });`

h: După câteva zile, dresorul crește volumul puțin câte puțin, până când câinele și-a depășit frica de tunete.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Se numește terapie prin expunere!

`hong({ body:"point", eyes:"normal" });`

h: Având în vedere că ești un câine, ar trebui să funcționeze și pentru tine, nu? Toate mamiferele au același răspuns de a lupta sau a fugi.

`hong({ body:"normal" });`

[Dacă ne desensibilizăm *prea* mult?](#act4_harm_exposure_overboard)

[Dacă suntem expuși unui pericol *real*?](#act4_harm_exposure_hurt)

[Sunt un lup, nu un câine.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Și îți voi arăta bunătate și răbdare până când vei fi domesticit într-un cățeluș micuț și drăguț.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Aww.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: *Tocmai* ce am văzut ce se întâmplă dacă îți ignori fricile: te poți pune în niște situații *într-adevăr* periculoase.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Pe lângă asta, nu cumva *prea* multă desensibilizare ne va transforma în psihopați?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: În curând ne vom recompensa în timp ce ne vom uita la porno dezgustător cu crime!

`hong({ eyes:"annoyed" })`

h: Cred... că este o limită dintre asta și un tunet.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Dar *unde* mai exact, omule? *Unde?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Nu știu. Dar *tu* mă poți ajuta!

`hong({ eyes:"normal", body:"normal" })`

h: Lucrând și negociind cu tine, vom trage acea linie.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: OK. Dar nu am degete mari opozabile, deci tu va trebui să o faci.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: De exemplu: am sărit de pe *acoperiș!*
{{/if}}

{{if !_.INJURED}}
b: De exemplu: aproape am sărit de pe *acoperiș!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Neh, ai dreptate. Oricine *poate* merge prea departe.

`hong({ eyes:"normal" });`

h: Dar de aceea, dacă facem terapia prin expunere, vom începe făcând niște pași mici înainte.

h: Tocmai înainte de a fi într-un *adevărat* pericol, ne vom opri.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Mda, trag linie dintre a auzi un tunet puternic și a sta într-o furtună purtând un coif ascuțit.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Stai așa, nimic de spus legat sau împotriva a ceea se simt? Doar un... „mulțumesc”?

`hong({ eyes:"surprise", body:"shrug" })`

h: Da! Îți mulțumesc de grija pentru {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Ești bine?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Nu mi-ai mai spus niciodată *mulțumesc* înainte.

`hong({ mouth:"smile" });`

h: Aww, lup pufos și speriat care ești.

(#act4_something_else)

# act4_thanks_2

h: Chiar dacă exagerezi, apreciez că ai grijă pentru {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Stai... nu repeți „mulțumesc” doar pentru a evita să vorbești despre acele frici, nu?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Păi, lucrurile sunt complicate, și nu am mereu răspunsuri pregătite.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Nu e ca și cum viața ți-ar da o listă de 3 răspunsuri pregătite.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Dar acum, pot măcar să îți mulțumesc.

b: Ei bine, și eu îți mulțumesc, pentru că m-ai ascultat cu răbdare.

`bb({ eyes:"closed" });`

b: Bucată de carne cheală și mică ce ești.

(#act4_something_else)

# act4_thanks_3

h: Chiar dacă lătratul tău mă sperie, încerci pur și simplu să-mi protejezi {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: OK, dacă mă mai flatezi atât, internetul își va face idei dubioase despre noi.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Hai măi, sunt doar un student vai de capul său, iar tu ești un lup mare și înfricoșător.

`hong({ eyes:"normal", body:"point" });`

h: De fapt, nu răspunde.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Vreau să fiu sigur că îți împlinești nevoia adâncă și umană de apartenență...

`bb({ eyes:"sad_u" });`

b: Dar mi-e teamă că dacă cineva ar ști de cine suntem noi *cu adevărat*, i-am face să dea bir cu fugiții.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Nu știu, gata cu alegerea *mea* pentru următoarea replică. Ce ai *tu* de spus, omule?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Din nou, înapoi la tine, omule. Ce crezi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Alte păreri, omule?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Sunt de acord, hai să lucrăm la viața noastră socială.](#act4_alone_skills)

[Cred că oamenii ne plac, hai să aflăm!](#act4_alone_experiment)

[Mulțumesc.](#act4_thanks) `_.thanks_for = "apartenența socială";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Am putea să practicăm abilități sociale: să punem întrebări, să ascultăm și să empatizăm, să fim deschiși și vulnerabili, etc?

`hong({ eyes:"normal_l" });`

h: Sau să ne facem obiceiuri sociale mai bune, cum ar fi să ieșim cu prietenii sau să mergem în mod regulat la întruniri?

`hong({ body:"one_up" });`

h: De asemenea, am putea învăța să fim mai confortabili cu refuzurile.

`hong({ eyes:"normal" });`

h: Sau să învățăm când oamenii *nu* ne resping, sunt doar obosiți sau așa e fața lor: încruntată.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Sunt multe opțiuni. Dar, legat de „învățarea abilităților sociale”...

[Nu-i asta *manipulare?*](#act4_alone_skills_manipulative)

[Nu ne va face asta să fim *mai ușor de manipulat?*](#act4_alone_skills_manipulated)

[Dacă încă vom eșua?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Nu sunt ucigașii în serie care pot citi emoțiile victimelor lor buni la „empatie”?

`bb({ eyes:"annoyed" });`

b: Nu-i așa că Charles Manson a câștigat prieteni și a înfluențat oamenii?

`hong({ eyes:"annoyed", body:"chin" });`

h: Mda, ai dreptate.

h: „Partea socială” nu înseamnă nimic dacă nu *ne pasă* cu adevărat de oameni.

`hong({ body:"normal" });`

h: Adică, doar nu fii un nesimțit/om de ^căcat^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Ăsta e un bun citat motivațional.

`hong({ body:"shrug", mouth:"narrow" });`

h: „Nu fii un nesimțit/om de ^căcat^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Vom deveni un preș de „Bine ai venit!” și vom spune „Te rog” și „Mulțumesc”, în timp ce oamenii își vor șterge picioarele de noi!

`bb({ mouth:"scream", eyes:"scream" })`

b: Vom pupa atât de tare în fund, vom părea că purtăm un ruj maro!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Neh, ai dreptate. „Abilitățile sociale” nu sunt doar pentru a face altora pe plac, trebuie să impunem și niște *limite*.
`hong( body:"one_up" });`

h: Nu-i putem invita pe alții în casa noastră, dacă nu avem pereți să o susțină.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Totuși... re: acea imagine mentală cu rujul... *iacs??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: S-ar putea să eșuăm... De fapt, *vom* eșua.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Și e în regulă! Din eșecuri se învață lucruri noi, în primul rând!

`hong({ body:"normal", eyes:"normal" });`

h: Deci hai să eșuăm împreună, bine?

`bb({ eyes:"normal_r" });`

b: OK, presupun... în cel mai rău caz, putem să fugim din orășel și să ne facem o nouă identitate.

`bb({ eyes:"normal" });`

h: Mda cred că asta costă, totuși, două bitcoin-uri în ziua de azi.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Am putea încerca niște experimente!

`hong({ body:"chin" });`

h: Am putea scrie unui prieten să ne întâlnim, să reluăm legătura cu un vechi prieten sau chiar doar să vorbim cu un barman.

`hong({ body:"normal" });`

h: Cred că ne vom da seama că suntem mai plăcuți decât ne așteptam.

`bb({ eyes:"annoyed" });`

[Dacă astea sunt „câștiguri” mici și nesemnificative?](#act4_alone_experiment_cheap)

[Daca asta e o povară pentru alții?](#act4_alone_experiment_burden)

[Dar discuțiile banale nu ne reprezintă pe *noi* ca persoane!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Dacă zâmbim superficial, nu vom avea niciodată legături sincere cu cineva,

`bb({ eyes:"super_sad" });`

b: *dar* dacă ne deschidem, alții vor vedea mizeria dinăuntrul nostru!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Rostogolește-te.

b: Ce.

`hong({body:"hands_1"})`

h: Când câinii vor să arate iubire și încredere, se fac vulnerabili prin a-și arăta burta.

`hong({body:"one_up"})`

h: Poate că nu ne simțim *încă* suficient de siguri să fim vulnerabili, dar cu suficient dresaj,

`hong({body:"normal", eyes:"surprise"})`

h: într-o zi le putem arăta oamenilor cine suntem cu adevărat: o dezordine, dar umană.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Mă voi rostogoli dacă îmi vei da o recompensă.

`bb({ eyes:"normal", mouth:"normal" });`

h: Nu.

(#act4_something_else)


# act4_alone_experiment_cheap

b: A saluta barmanul nu e o perfomanță de o medalie de aur la Olimpiada de Socializare.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Pentru *noi* este!

`hong({ body:"one_up", eyes:"annoyed" });`

h: În arena socială, nu suntem nici măcar la nivelul unei pene, suntem precum... o moleculă.

`hong({ body:"normal", eyes:"normal" });`

h: Dacă trebuie să începem cu câștiguri mici și nesmnificative, așa să fie. Trebuie să urcăm prima treaptă înainte de a ajunge la a o mia.

b: Da! Poate după ce salutăm, putem avansa la a întreba... 

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *„Ce mai faci?”*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *„Nimic interesant!”*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Poate barmanul doar vrea să facă o amărâtă de cafea, nu să fie un cobai pe care să ne testăm abilitățile de comunicare.

`bb({ eyes:"annoyed" })`

h: Păi, și dacă până la urmă *suntem* o povară...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: E și asta bine de știut!

`hong({ eyes:"normal" });`

h: Putem apoi să învățăm cum să întrebăm lumea de nivelul lor de confort, pentru a le ști și respecta limitele.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Știi, tot ^rahatul^ ăsta cu „abilitățile inter-personale” pe care le vedem în broșurile consilierilor.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Vreau să-ți apăr nevoile morale, acel impuls de a deveni o persoană mai bună,

`bb({ eyes:"sad_d" })`

b: dar se simte de parcă, în adâncul nostru, suntem atât de... stricați.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: Și să nu-mi spui că *nu* suntem stricați. Am sărit de pe un *acoperiș*.
{{/if}}

{{if !_.INJURED}}
b: Și să nu-mi spui că *nu* suntem stricați. Aproape că am sărit de pe un *acoperiș*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Nu știu, gata cu alegerea *mea* pentru următoarea replică. Ce ai *tu* de spus, omule?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Din nou, înapoi la tine, omule. Ce crezi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Alte păreri, omule?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Deci, suntem stricați. Hai să ne reparăm.](#act4_bad_fix)

[Deci, suntem stricați. Hai să acceptăm asta.](#act4_bad_accept)

[Mulțumesc.](#act4_thanks) `_.thanks_for = "bunăstarea morală";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Am putea construi încet-încet niște obiceiuri mai bune, să ne aliniem viața cu valorile noastre,

`hong({body:"one_up"});`

h: iar dacă va fi nevoie, putem primi ajutor de la profesioniști: un terapeut sau un consilier.

`hong({body:"normal"});`

h: Sunt căi pentru a ne repara.

[Dacă nu putem repara tot?](#act4_bad_fix_cant)

[Dacă reparăm *prea* mult?](#act4_bad_fix_too_much)

[Nu ne putem permite ajutor profesional.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Neh, presupun că ai dreptate.

h: Nu putem repara tot.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: AAAAAA știam eu că vom fi mereu stricați!

`hong({eyes:"surprise"});`

h: Dar măcar putem fi *mai puțin* stricați.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Cicatricile se vindecă cu timpul, dar nu dispar niciodată. Și e în regulă.

`bb({eyes:"annoyed_r"});`

b: Presupun. Pe lângă asta,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Cicatricile sunt *sexy.* 

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Te rog, nu face asta.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Se simte nebunesc să recunosc, dar parcă... o parte din mine *ar vrea* să aibă această tulburare.

`bb({ eyes:"angry" })`

b: Adică, fără ea, n-am fi cumva *plictisitori?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Fără boală, n-ar deveni arta noastră anostă și insipidă?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Fără boală, ne-am mai putea apropia de prietenii noștri care au tulburarea?

`bb({ eyes:"sad", body:"chest" })`

b: Dacă vom fi mulțumiți cu viața noastră, nu cumva ne vom opri motivația de a face chestii grozave?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Chiar dacă ne e frică... „să rămânem fără frici”...

h: Nu cred că vom rămâne vreodată fără frici.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Ah, da! Ce ușurare!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: „Doctore, sunt anxios că plătesc 400 RON/oră doar să te aud întrebându-mă *cum te face să te simți?*”

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: „Aha. Și asta cum te face să te simți?”

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Neh, ăsta e un motiv rezonabil de îngrijorare.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Și sincer, e nașpa că sistemul de sănătate mentală nu este accesibil pentru multă lume.

`hong({ eyes:"normal", mouth:"normal" });`

h: Totuși, există niște alternative ieftine sau gratis:

`hong({ body:"chin" })`

h: Grupuri de suport, terapie online, centre de sănătate studențești/non-profit...

`hong({ body:"hands_1" })`

h: Construirea unor obiceiuri precum meditația, dormitul bine, discuții periodice cu prietenii, învățarea unor lucruri noi...

`hong({ body:"hands_2" })`

h: Mersul la o bibliotecă pentru a împrumuta manuale de psihoterapie bazată pe dovezi...

`hong({ body:"one_up" })`

h: Este o listă completă de resurse la sfârșitul acestui joc!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Ei bine, *acea* a patra parte n-a durat prea mult.

`hong({ body:"point" });`

h: Câteva lucruri sunt mai importante decât o convenție narativă. Cum ar fi sănătatea mentală.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Adică, asta spun toți terapeuții, corect? Să ne acceptăm emoțiile, chiar și pe cele negative?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Stai.

[„A accepta”, adică *a renunța*?](#act4_bad_accept_give_up)

[„A accepta” adică *a fi de acord*?](#act4_bad_accept_approve)

[„A accepta” adică *să le luăm în serios*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Crezi că Martin Luther King ar fi zis, "Nășpik că nu putem sta în față în autobuz, hai să *acceptăm* asta?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: De ce cei de la Complexul Industrial de Dezvoltare Personală cred că fluturarea steagului alb este ceva *înțelepciune profundă?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Cred că terapeuții se referă la „a accepta” lucrurile rele prin a lua la cunoștință că există și că sunt greu de schimbat,

h: Dar nu înseamnă neapărat să renunți la angajamentul pentru schimbare.

`bb({ eyes:"suspect" });`

b: Păi atunci, terapeuții ar trebui să spună *a lua la cunoștință*, nu *a accepta*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Da, acum că mă gândesc mai bine, „a accepta” e cam derutant.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Păi, *am luat asta la cunoștință*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: De parcă ar fi *bine* că suntem stricați sau ceva? Nu!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Toți scenariștii ăia blestemați de la Hollywood care glorifică bolile mentale sunt plini de ^rahat^!

`bb({ eyes:"angry", body:"two_up" });`

b: E *nașpa* să ai o tulburare mentală! Jefuiește oamenii de *vieți!* De ce ar trebui să „acceptăm” asta?!

`bb({ body:"normal" });`

h: Cred că terapeuții se referă la „acceptarea” emoțiilor prin a avea răbdare cu ele.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: La fel cum dacă te miști într-un nisip mișcător te face să te îneci mai repede, iar soluția este să fim întinși răbdători pe spate,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Lupta împotriva ta, frica mea, m-a făcut să mă arunc de pe acoperiș.
{{/if}}

{{if !_.INJURED}}
h: Lupta împotriva ta, frica mea, aproape că m-a făcut să mă arunc de pe acoperiș.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: În schimb, soluția este să facem ceea ce facem acum: nu să ne certăm, ci să fim răbdători unii cu ceilalți.

`bb({ eyes:"annoyed" });`

b: Atunci ar trebui să zică *asta* în loc de un cuvânt problematic precum „a accepta”.

`hong({ body:"chin", eyes:"annoyed" });`

h: Mda, acum că mă gândesc la asta, „a accepta” e cam nașpa.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Nu accept „acceptarea”.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Dar deja *știi* că nu ar trebui să mă iei în serios!

`bb({ eyes:"sad_u", body:"two_up" });`

b: *Problema* este că aș vrea să te ajut, dar sunt nașpa la folosirea cuvintelor cu scopul ăsta!

`bb({ eyes:"sad", body:"normal" });`

h: Cred că terapeuții se referă la „acceptare” prin „a nu te împotrivi sau a nu le ignora”.

`hong({ eyes:"surprise", body:"one_up" });`

h: Să te asculte, să lucreze *cu* tine, dar să nu ia ceea ce spui ca fiind 100% adevărul absolut.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Atunci terapeuții ar trebui să spună *asta* în loc să folosească cuvinte vagi și derutante precum „a accepta”.

`hong({ body:"chin", eyes:"annoyed" });`

h: Presupun că și ei sunt nașpa la folosirea cuvintelor.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Mă rog, altceva despre care ai vrea să discutăm?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Așadar, mai ai ceva pe sufletul tău mare?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Mi-e teamă să fim răniți.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Mi-e teamă să rămânem singuri.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Mi-e teamă de a fi niște oameni răi.](#act4_bad)
{{/if}}

[Neh, e ok momentan.](#act4c_prelude)

# act4_something_else_2

h: OK, cred că am vorbit despre toate temerile noastre acum.

b: Da, aici sunt doar trei temeri.

h: Dap, fix trei.

b: Convenabil.

(#act4c)

# act4c_prelude

h: Bună discuție, echipă.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Ăsta nu e doar un *joc*, să știi.

`bb({eyes:"angry_d", body:"one_up"})`

b: Să construiești o relație sănătoasă cu emoțiile tale nu este așa de simplu precum apăsarea unor butoane de pe ecran. 

`bb({eyes:"sad", body:"normal"})`

b: Chiar *putem* să ne înțelegem?

b: Chiar *putem* lucra împreună, ca o echipă?

`hong({eyes:"sad", body:"one_up"})`

h: Ei bine,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: S-scuză-mă... 

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: A-a-ar fi în regulă să stau cu tine la prânz?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Asta* e persoana pe care o placi? De ce stă singur ca un criminal în serie psihopat?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Să o întrebi pe persoana pe care o placi dacă putem sta cu ea? Știi cât de *disperați* părem?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Asta* e persoana pe care o placi? I-am întrerupt liniștea și pacea! Suntem o așa povară!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: A-adică e, e în regulă dacă nu, doar...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Stai, nu cumva te-am văzut la petrecere?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Da, desgigur! Vino aici.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Scuze, am nevoie să fiu singur acum.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Da, erai pe canapea! La prima petrecere la care am fost...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Unde am avut atacul ăla de panică și i-am dat un pumn gazdei.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Unde am avut atacul ăla de panică și am fugit plângând.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Stai puțin, omule, poate o facem să se simtă inconfortabilă.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Aaa, nu vreau să te pun într-o situație jenantă!

`publish("act4", ["hong_to_alshire",4]);`

h2: Doar mi-am amintit de cineva cunoscut, atât.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AAAAA, ȘTIAM EU! ESTE UN NEBUN PERICULOS CARE SE LASĂ CONDUS DE PANICĂ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAAAA PRIMA IMPRESIE PE CARE AM FĂCUT-O A FOST „MARTORII TRAUMEI MELE”! ÎNSEAMNĂ CĂ NE URĂȘTE!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAAAA AM FĂCUT PE CINEVA SĂ-ȘI AMINTEASCĂ DE UN EVENIMENT TRAUMATIZANT. SIMPLA PREZENȚĂ A NOASTRĂ ÎI RĂNEȘTE PE CEILALȚI.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Stai puțin, omule, poate o facem să se simtă inconfortabilă.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: A, fără presiune desigur!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Zic doar că poți sta aici dacă vrei.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ESTE *PREA* PRIETENOASĂ! PRECUM TED BUNDY, CRIMINALUL ÎN SERIE!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: DOAR SE COMPORTĂ DRĂGUȚ CU NOI! NIMENI NU *PREA* VREA SĂ SE APROPIE DE NOI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAA ÎI FACEM PE ALȚII SĂ SE SIMTĂ STÂNJENIȚI! SUNTEM O PATĂ PE PĂMÂNT!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Stai puțin, omule, poate o facem să se simtă inconfortabilă.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: A, nu am vrut să fiu nașpa!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Doar am nevoie să-mi procesez emoțiile. Te rog să nu o iei ca pe o respingere.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: CE GÂNDURI BOLNAVE ȘI SUCITE PROCESEAZĂ?! CE DORINȚE ÎNTUNECATE ÎI UMPLE INIMA ACESTUI PSIHOPAT?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AM FOST RESPINȘI! NU VOM FI NICIODATĂ IUBIȚI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: LE-AM ÎNTRERUPT PROCESUL EMOȚIONAL! ACUM VA FI TRAUMATIZAT PENTRU TOTDEAUNA ȘI E DOAR VINA NOASTRĂ!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI FUGI

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Hm. A fost ciudat. Mă întreb ce se întâmpla în mintea sa.

`publish("act4", ["hong_closer", 2]);`

h: Mă rog, ce ziceai?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, am uitat? Ceva legat de echipe și muncă?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Se spune că trebuie „să faci pace” cu emoțiile tale, de parcă emoțiile ar fi *criminale de război*.

`publish("act4", ["bb_closer", 7]);`

b: Dar vreau să fie între noi *mai mult* decât pace! Aș vrea să fim *aliați!* But I want us to make *more* than mere peace! I want us to be *allies!*

`publish("act4", ["bb_closer", 3]);`

b: Aș vrea să fiu un câine de pază bun. Precum foamea și setea sunt alarme pentru neoile tale fizice... I want to be a good guard-dog. Just like how hunger & thirst are alarms for your physical needs,

`publish("act4", ["bb_closer", 8]);`

b: Vreau să fiu alarma pentru nevoile tale *psihologice* - nevoile tale de siguranță, apartenență, bunătate.

`publish("act4", ["bb_closer", 1]);`

b: Dar... sunt nașpa la asta, deci am nevoie de tine pentru a mă dresa.

`publish("act4", ["bb_closer", 4]);`

b: Nu „am mereu dreptate”, nici nu stunt „irațional” mereu. Încerc doar... să dau tot ce-i mai bun din mine. Deci, te rog...

`publish("act4", ["bb_closer", 30]);`

b: Ajută-mă să te ajut!

`publish("act4", ["bb_closer", 6]);`

b: Deși, să înveți un câine bătrân trucuri noi *va lua* ceva timp. Poate chiar *ani*.

`publish("act4", ["bb_closer", 3]);`

b: Și câteodată voi recidiva, voi aluneca spre vechiile mele obiceiuri.

`publish("act4", ["bb_closer", 2]);`

b: Voi lătra la umbre. Te voi speria cu cuvinte. Poate chiar am să-ți arăt niște imagini intruzive cu... chestii.

`publish("act4", ["bb_closer", 9]);`

b: Îmi pare rău! Sunt un câine de adăpost schingiuit! Câinii schingiuiți mai fac caca în patul tău câteodată!

`publish("act4", ["bb_closer", 4]);`

b: Dar dacă ai răbdare cu mine... și vei sta cu mine... But if you're patient with me... and just stay and sit with me...

`publish("act4", ["bb_closer", 8]);`

b: Poate poți îmblânzi acest lup.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bun câine.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Bun om.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA ÎNCĂ MĂNÂNCI SINGUR CINCISPREZECE ȚIGĂRI AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA ÎNCĂ NU EȘTI PRODUCTIV ÎN TIMP CE MĂNÂNCI SUNTEM NIȘTE PARAZIȚI SOCIALI AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA MĂNÂNCI MAI MULTĂ PÂINE ALBĂ AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: HAM HAM HAM HAM HAM

(#credits)
