# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Dar tu ai *văzut* "știrea" aia despre lucrul acela înfiorător care s-a întâmplat undeva?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: s-sal...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Urăsc știrile. Nu sunt decât senzaționalism și clickbait..

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: f... faină petrecere...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Așa e, dar nu fac decât să răspundă cererii. *Adevărata* problemă sunt oamenii care dau click.

```
publish("act2",["dee",3]);
```

s: Cine ar distribui o știre înfiorătoare să-și facă toți prietenii să se simtă de ^căcat^?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, așa-i?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Dar ai *văzut* cum a devenit virală "știrea" aceea?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: s-salu...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Da, complet falsă. Cine s-ar lasă păcălit de așa ceva și ar redistribui-o??

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: f... faină petrecere...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Pe bune frate. Deschide și tu Google și verifică sursele când vezi așa ceva?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, știu, așa-i?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: După cum ziceam, Complexul Industrial Pentru Meme-uri exploatează pisicile.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: s-salu...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Okay, elaborează această ipoteză.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: f... faină petrecere...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Păi am văzut că cineva a redistribuit un GIF ieri cu o pisică care bea lapte.

```
publish("act2",["dee",3]);
```

s: Pisica nu poate digera laptele! Cine ar redistribui un act de *abuz împotriva unui animal*?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, știu, așa-i?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: Mda, și nu mi-au mai răspuns!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: s-salu...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Chiar dacă aveați match pe Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: f... faină petrecere...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Da, chiar dacă! Ce și-o fi imaginat, că sunt vreun criminal în serie sau ceva? Super paranoic.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, știu, așa-i?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Da, nu știu. Poate ei cred că întâlnirile casual nu le poate umple golul din suflet?

s: Nu mai fi așa mironosiță! Deschide-ți mintea mai întâi, și apoi picioarele!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, știu, așa-i?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Da, nu știu. Nu erau cine știe ce dar n-ar fi fost o partidă rea.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Trebe Prinși Toți!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: RUNDA A DOUA: *LUPTĂ!*

[Oh nu toată lumea ne urăște!](#act2a_social)

[Te *holbai* la roșcată?](#act2a_perv)

[Hey, hai să vorbim despre sensul vieții.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stricăm cheful tuturor cu starea asta negativă!

`bb({eyes:"shock", body:"two_up"})`

b: Omorâm bună dispoziție! Comitem crimă de gradul 1, distrugem vibrațiile pozitive!

`bb({eyes:"normal", body:"normal"})`

b: Trebuie să plecăm *acum*, omule, înainte să--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Arată mai bine decât noi, ceea ce înseamnă că dacă doar ne *uităm* în direcția lor, atunci--

`bb({eyes:"shock", body:"two_up"})`

b: SUNTEM DUBIOȘI

`bb({body:"normal"})`

b: Suntem niște dubioși siniștri, perverși oribili și răi, răi foarte răi--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: În final și la urma urmei, ce putem face noi să conteze cu adevărat? 

`bb({body:"normal", eyes:"sad"})`

b: Să contribuim cu ceva? Orice-am face se duce pe calea lui Ozymandias. Iubire? Moartea ne va despărți.

`bb({eyes:"sad_r"})`

b: Și câtă moarte e peste tot! Și *noi* vom muri. Toți *oamenii pe care îi iubim* vor muri..

`bb({eyes:"shock", body:"two_up"})`

b: Rahat, conform celei de-a două legi a termodinamicii, până și *universul* va muri!!

`bb({eyes:"suspect", body:"normal"})`

b: Ah, "moartea ne face să apreciem viața"? Asta e ca și cum ai spune că sclavia e bună pentru că ne face să apreciem libertatea!

`bb({body:"one_up"})`

b: Ah, "trebuie să îți construiești singur sensul"? Asta fac numai cultele și conspiraționiștii!

`bb({eyes:"shock", body:"two_up"})`

b: Viața nu are nici un sens, moartea nu are nici un sens, nici măcar *sensul* nu are nici un sens! Ce poate un biet suflet de muritor să--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Hm... mă auzi, omule?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *GASP*

`bb({mouth:"small_talk"})`

b: AR TREBUI SĂ TE AVERTIZEZ DESPRE...

[Același pericol, dar mai *mare* !](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *alt* pericol social!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *alt* pericol moral!](#act2b_different_moral)
{{/if}}

[Ignori pericolul! Asta e periculos!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: EMOȚIILE SUNT CONTAGIOASE! AȘA CĂ DACĂ NU PLECI ACUM, ÎI VEI INFECTA PE TOȚI CU BOALA TA MENTALĂ! 

b: Vei provoca o epidemie mortală de SINDROMUL VARZĂ TRISTĂ

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Trebuie să plecăm de aici și să intrăm la izolare la noi în cameră cu Netflix și cu mâncare livrată la ușă!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NU FI DUBIOS. E ILEGAL!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Legea Dubioșilor, Secțiunea 74.5: (1) Orice Persoană care se uită prea lung la (a) umerii aceia musculoși (b) fundul acela bombat (2) va fi recunoscută drept

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UN PERVERS DUBIOS DEZGUSTĂTOR"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: De fapt, chiar și dacă îți găsești un scop nobil în viață, *tot* poți strica totul!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel și-a dorit pace-n lume și ca toate culturile să se înțeleagă. Așa că a vrut să ușureze călătoritul.

`bb({eyes:"normal_r"})`

b: Și pentru asta avea nevoie să creeze tunele cât mai ieftin. Așa că a inventat un nou material numit "dinamită"...

`bb({body:"one_up", eyes:"normal"})`

b: care a fost folosit în primul război mondial că să OMOARE MILIOANE DE OAMENI

`bb({body:"two_up", eyes:"shock"})`

b: E EFECTUL FLUTURE, NU-L ȘTII? TU CÂȚi OAMENI CREZI CĂ OMORI CHIAR ACUM DIN GREȘEALĂ?

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: De fapt știi ce e și mai rău decât să nu te placă nimeni? Să te placă *toată lumea*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Adică să devii un animal din *ăsta* care trăiește să îi mulțumească pe ceilalți.

`bb({body:"normal", mouth:"small"})`

b: O viață superficială cu prieteni superficiali care te cunosc superficial.

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Trebuie să fugim de zombie ăștia hedoniști înainte să ne transforme și pe noi într-unul din ei!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Oameni mor *chiar acum* de foame și în genociduri și noi petrecem!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un înțelept a spus o dată că "singurul lucru necesar pentru ca răul să triumfe este ca oamenii buni să nu facă nimic".

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NU FACEM NIMIC.

`bb({mouth:"small"})`

b: DISTRANDU-NE, ÎL AJUTĂM PE *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Crezi că ești în siguranță doar pentru că ai scos bateriile din detectorul de monoxid de carbon?

`bb({eyes:"suspect_r"})`

b: Nici măcar nu o să simți otravă! Ți se va face numai foarte somn și apoi o să--

`bb({body:"scream_c_1"})`

b: MOOOOOOOOOOOOORI

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Slavă cerului, cred că mă poți auzi din nou!

`bb({eyes:"closed", body:"point"})`

b: AM SĂ TE AVERTIZEZ DESPRE...

{{if _.a2_first_choice=="louder"}}
[*Încă și mai mult* din același pericol!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Mai mult* din același pericol!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Un *alt* pericol social!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *alt* pericol moral!](#act2c_different_moral)
{{/if}}

[Tu ai verificat lichiorul acela înainte să bei din el?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: De fapt Netflix și mâncare livrată la ușă nu e o carantină eficientă! Am putea infecta curierul!

`bb({body:"one_up", mouth:"small"})`

b: Ce trebuie făcut e să ne mutăm în teritoriile Yukon din Canada și să ni se livreze mâncarea cu drona!

`bb({body:"two_up", mouth:"normal"})`

b: Și apoi drona va trebui să fie sterilizată să nu mai rămână nici o urmă din microbii de Varză Tristă

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Perversul DUBIOS  DEZGUSTĂTOR va primi drept pedeapsă 72 de ore într-un dispozitiv din acela de umilire publică

b: în afară de cazul în care în secret *îi face plăcere* genul ăsta de chestie

`bb({body:"scream_a_1"})`

b: pentru că e un PERVERS DUBIOS ABSOLUT DEZGUSTĂTOR

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFECTUL FLUTURE! Folosești un pahar din plastic ne-biodegradabil?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, UN DEȘEU ELIMINĂ UN GAZ OTRĂVITOR ȘI OMOARĂ UN COPIL

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Transpiri și îți bate inima foarte tare?

`bb({body:"scream_a_1"})`

b: BAM, NE RUINEZI SISTEMUL DE SĂNĂTATE ȘI MOR MILIOANE DE OAMENI

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Zombie hedoniști te vor înconjura șoptind printre dinți

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: LIIIIIKE-URI. LIIIIIIIIIIKE-URI.

`bb({body:"scream_a_1"})`

b: Apoi te vor mușca și te vor transformA într-un COAE FĂRĂ CREIER și/sau într-o FATĂ FRAIERĂ!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: NAZIȘTII AU IEȘIT IAR SĂ MĂRȘĂLUIASCĂ PE STRĂZI CHIAR ACUM

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Spunând *super bine că toți oamenii de treabă s-au relaxat și se preocupă cu wellness-ul și sănătatea mentală!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Acum ne putem vedea de planuri liniștiți, taman la timp!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: De fapt dacă stau bine să mă gândesc, știm dacă clădirea asta *are* totuși detector de monoxid de carbon?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: Dacă suntem de fapt cu toții otrăviți chiar *ACUM*?

`bb({body:"scream_a_1"})`

b: NICI NU AM SIMȚI MOARTEA APROPIINDU-SE. PUR ȘI SIMPLU AM ÎNCETA SĂ EXISTĂM, PENTRU TOTDEA--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: Și dacă suntem *fundamental incapabili* de a fi vreodată iubiți, sau de a iubi pe altcineva?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Dacă s-a stricat ceva iremediabil în noi acum multă vreme? Sau dacă nici nu a existat vreodată?

`bb({body:"scream_a_1"})`

b: AHH SUNTEM STRICAȚI! ATÂT DE STRICAȚI, ATÂT DE STRI--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Și dacă suntem *fundamental stricați* pe dinăuntru?

`bb({body:"one_up", eyes:"sad"})`

b: Alții fac bine din instinct dar noi nu facem bine decât din teamă, vină sau rușine.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Dacă e în natură noastră să îi ranim pe ceilalți ? Dacă nu putem fi nimic *altceva* în afară de o povara pentru apropiați?

`bb({body:"scream_a_1"})`

b: AHH SUNTEM STRICAȚI! ATÂT DE STRICAȚI, ATÂT DE STRI--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Nu sunt irațional deloc. *Chiar* se practică pusul drogurilor în băuturi. Este absolut ceva ce se întâmplă.

`bb({eyes:"suspect"})`

b: Auzi, nu te doare capul? Ți s-au înmuiat cumva picioarele? Cred că murim.

`bb({body:"scream_a_1"})`

b: AHHH MURIM! MURIM MURIM MURIM MURIM MURIM MU--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: P^UUULA^!

h: P^UL^A P^UL^II -P^IZD^IIII *P^ULIIIIII^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Yay, ooom! Ce mă bucur că mă auzi din nou!!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: De ce mă ignorai adineaori?

`hong({body:"facepalm"})`

h: Rahat împrăștiat, cretin idiot!

`hong({body:"facepalm_2"})`

h: Știi povestea aia amerindiană?

h: "Sunt doi lupi înăuntrul tău: unul e speranța, altul e disperarea. Ce lup câștigă? Cel pe care îl hrănești."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Încercam să te *înfometez*, ^cretin^ sadic!

`hong({body:"smile", mouth:"smile"})`

h: În fine, am să încerc afirmații pozitive, poate merg.

h: *Sunt iubit. Sunt bun. Sunt deștept. Sunt frumos. Sunt special.*

`bb({eyes:"suspect"});`

[Wow, ce super narcisist!](#act2d_narcissist)

[Știi că tehnica afirmațiilor *nu e dovedită*?](#act2d_disproven)

[Nu atribui povești aleatorii populațiilor indigene!](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Poate de fapt să *dăuneze* oamenilor care au deja încredere scăzută în ei înșiși! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Studiul e foarte bine formulat - experiment randomizat controlat, conducătorul experimentului nu știe grupul alocat subiectilor.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Rezultate: dacă îți spui afirmații pozitive când ai încrederea scăzută în tine, te vor face să te simți *mai prost* decât dacă nu spuneai nimic!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Științe Sociale. Caută studiul pe Google Scholar, omule,

`bb({body:"scream_b_1"})`

b: ȘI APOI OPREȘTE-TE DIN A DITRIBUI INFORMAȚII FALSE NEDOVEDITE ȘTIINȚIFIC

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Este *necesar* să îți privești cu umilință propriile defecte pentru a putea crește că persoană!

`bb({body:"two_up", eyes:"suspect"})`

b: Nu poți să pui odorizant într-o cameră cu mucegai pe pereți! E mai rău pe termen lung să îți acoperi și să îți negi defectele.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Din fericire ca lupoiaca ta de pază îți pot arată eu defectele. Și în momentul asta, astea sunt--

`bb({body:"scream_b_1"})`

b: TOT. TOTUL E GREȘIT. NIMIC NU E BINE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Populația indigenă a Americii este formată din *oameni adevărați*, nu sunt niște sălbatici nobili la care să faci referire că să îți sune sfaturile mai *exotic*.

`bb({eyes:"suspect_r"})`

b: Reduci întregi culturi la mesaje simpliste de pus pe felicitări Hallmark! Știi cum se cheamă asta: "rasism benevolent"!

`bb({body:"scream_b_1"})`

b: OPREȘTE-TE DIN A FI UN RASIST NESIMȚIT

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^RAHAT^.

`hong({body:"yell", mouth:"yell"})`

h: Știi ceva, ești *irațional*.

h: Toată lumea știe că emoțiile sunt iraționale. Mai ales frica!

`hong({body:"facepalm_2"})`

h: Ești o rămășiță evoluționară inutilă, ca apendicele sau ca măselele de minte!

`hong({body:"yell", mouth:"yell"})`

h: Și metaforă asta cu lupul e stupidă! Nu ești decât un cocktail de neuro-chimicale din creierul meu.

`hong({body:"cross", mouth:"cross"})`

h: Așa că de ce ar trebui să ascult de o mizerie inutilă, irațională, non-existentă??!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Jeez, omule. M-a durut rău asta.](#act2e_hurtful)

[Sunt un sentiment. Sentimentele sunt valide.](#act2e_valid)

[Omule. Suntem *amândoi* "doar niște chimicale."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Sunt o *parte* din tine, să știi. Când spui asta, pe tine insuți te faci să suferi.

`bb({body:"scream_a_1"})`

b: De ce te lovești singur, omule? NU TE MAI AUTOFLAGELA.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Motivațiile tale intrinseci sunt doar dopamină, bucuriile tale cele mai bogate sunt serotonină.

`bb({body:"one_up"});`

b: Amintirile tale sunt greutăți sinaptice, rațiunea ta este o rețea de semnale electrice.

`bb({eyes:"normal", body:"normal"});`

b: Așa că dacă *eu* sunt irațional pentru că sunt doar chimicale.. atunci și *tu* ești irațional!

`bb({body:"two_up", eyes:"shock"});`

b: Și dacă suntem *amândoi* iraționali, n-o să reușim *niciodată* să fim fericiți și împliniți!

`bb({body:"scream_a_1"})`

b: AHHH SUNTEM STRICAȚI! ATÂT DE STRICAȚI, ATÂT DE STRI--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Deci "se spune" că sentimentele sunt valide, și că ar trebui mereu să îți accepți emoțiile.

`bb({eyes:"suspect_r"});`

b: Dar "se spune" *și* că emoțiile sunt iraționale, și că să nu ai încredere în ele.

`bb({eyes:"angry"});`

b: Suntem mințiți, am fost mereu mințiți!

`bb({body:"scream_a_1"})`

b: NI SE BAGĂ PE GÂT CONTRADICȚII CĂ SĂ NE FACĂ DEPENDENȚI DE INDUSTRIA DE PRODUSE DE AUTO-AJUTORARE

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: E oribil. Doare atât de tare, *urăsc* să mă simt așa.

h: Nu te pot mulțumi. Nu te pot ignora. Nu te pot bate. 

`bb({eyes:"suspect"});`

h: Nu reușesc să scap de tine indiferent de ce încer--

`bb({body:"cry_1"});`

b: Atunci poate că *NU AR TREBUI* SĂ SCAPI DE MINE.

`bb({body:"cry_2"});`

b: Și *eu* cum crezi că mă simt, hmm?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Încerc din răsputeri să te apăr, ca un câine bun de pază, dar indiferent ce fac tu mă vezi Lupul Cel Rău!

b: Așa că încerc și mai tare să îți arăt ce pericol te paște! Un pericol mai mare! Un pericol diferit!

`bb({eyes:"cry_2"})`

b: Dar indiferent cât de tare încerc să te protejez, tu tot ca pe-un dușman mă privești!

`bb({body:"cry_5"});`

b: Ce fac greșit?!

`bb({body:"cry_2"});`

b: *Știu* că nu sunt deloc bun la ce fac. Dar *încerc*, omule!

`bb({body:"cry_3"});`

b: ...încerc.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Nu trebuie să ții seama de ce zic, sau să fii de acord cu mine, sau să mă *placi*.

`bb({eyes:"cry_r_2"});`

b: Vreau doar.. tot ce vreau e să ai puțină răbdare cu mine.

`bb({eyes:"cry_r_3"});`

b: Vreau doar să stai puțin cu mine, în loc să-mi întorci imediat spatele și----

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hey.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Pare că ești prins într-o luptă cu tine însuți puștiule.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Așa evident e?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Pai, uhm, mormăiai singur aici despre {{_.a2_hoodie_callback}} sau ceva.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: oh doamne sunt jalnic.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Nu ești singur, prietene. Anxietatea e foarte comună.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Chiar ieri am auzit că cineva a avut o cădere nervoasă în campus și și-a spart telefonul de ciment!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Chiar ieri am auzit că cineva a avut o cădere nervoasă în campus și a plâns în hohote în public!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Pe bune, știu cum e să ai animalul acela în cap tot timpul.

```
publish("act2",["party_hunter",8]);
```

r: Cu *toții* știm. Eu de asta organizez petrecerile astea în fiecare weeekend, că să uităm de griji, să uităm de animalul ăla.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: dar anxietatea mea...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Nu-ți fă griji puștiule. Și eu am fost că tine. Dar am descoperit ceva ce m-a ajutat să opresc vocea aia negativă pentru totdeauna...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: Amestecul meu special. E un pic mai tare decât.. hmm decât cam orice e legal.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Până la fund, ^muică^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Doamne ferește.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Asta e o soluție proastă de făcut față.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Nu accepta băuturi de la străini.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, ce gust rafinat!

h: O aromă rotundă, plină de "oprește-ți gândurile", urmată de un gust ulterior subtil de "nu mai simți niciodată nimic"!

b: Nu e okay, omule. Nu e deloc, deloc okay.

[Asta este *literal* cum se declanșează adicția.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[*Știam* eu că gazda este absolut dementă!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Plus că poate să fi pus și droguri în băutură!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: Asta este *lite*--

(#act2h)

# act2h_opt2

b: Plus că poa--

(#act2h)

# act2h_opt3

b: *Știam* eu că--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Delicios *și* mai ieftin decât terapia!

b: OPREȘTE-TE TE ROG

h: Hehehe!

h: Altfel ce, ce-o să faci *tu* ^muistule^?

b: Îmi pare atât de rău, omul meu.

b: Va trebui să îmi folosesc ARMA SECRETĂ.

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Despre ce căcat vorbești?

h: O să scuipi și mai multe *vorbe* înspre mine ca--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CE ^NAIBA^ A FOST ASTA

b: Îmi pare rău. A trebuit să îți arăt consecințele.

{{if _.SPECIAL_ATTACK=="harm"}}
h: MI-AM PUTUT *VEDEA* PROPRIUL CADAVRU. AM PUTUT *SIMȚI* CUM E SĂ FII PE BUNE MORT.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: AM PUTUT *VEDEA* PRIVIREA DE DEZGUST A TUTUROR. AM PUTUT *AUZI* TOT CE ZICEAU DESPRE MINE.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: AM PUTUT *AUZI* CUM SE RUP COASTELE. AM PUTUT *SIMȚI* SÂNGELE ÎN AER.
{{/if}}

b: Îmi pare rău, omul meu.

n: *DĂ-I LOVITURA DE GRAȚIE*

[{ATACĂ: Da-i o palmă gazdei.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{PLEACĂ: Hai să plecăm de-aici.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Psihopatul ăsta încerca să profite de tine..

b: Încerca să te corupă, să te facă la fel de distrus că și el!

`bb({ body:"yell_angry_1" });`

b: Pocnește-l! Dă-i una să nu se mai ridice!

`bb({ body:"final_1" });`

b: POCNEȘTE-L POCNEȘTE-L POCNEȘTE-L POCNEȘTE-L POCNEȘTE-L POCNEȘTE-L POCNEȘTE-L POCNEȘTE--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: *Știam* eu că ăștia care merg la petrecerile astea sunt profund distruși. Încearcă să-și înnăbușe durerea cu chestii nasoale!

`bb({ body:"yell_1" });`

b: Și te fraieresc să faci și tu același lucru! Te corup! Tre să ieșim de-aici! Pleacă acum.

`bb({ body:"final_1" });`

b: PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEACĂ PLEA--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Ești ok, puștiule?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: Eș-ești...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: ești *kinky*.

r: Îmi placi. Hai la petrecerea mea weekendul viitor, păpușă.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok pa pa, ciao, adios, au revoir

r: Poate că astăzi a câștigat animalul, dar să te întorci, fac un amestec încă și mai tare pentru tine!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Tu și cu mine, puștiule, îi arătăm noi animalului cine e șeful!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok sorry tre sa plec

`publish("act2",["party_hunter",16]);`

r: La ^naiba^. A câștigat dihania azi, huh?

`publish("act2",["party_hunter",15]);`

h2: nu nu, doar că, uh, am un maraton la care fug. tre să fug.

`publish("act2",["party_hunter",19]);`

r: Vino la petrecerea de weekendul viitor păpușă, îți fac un amestec și mai tare, doar ție.

h2: ok mersi tre să fug să fug să fug să fug

r: Tu și cu mine, puștiule, îi arătăm animalului cine e șeful!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Omul meu! Ești okay?!

```
publish("act2", ["act2_end","next"]);
```

b: A fost cam *la mustață*. Puteam să--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Weekendul viitor mă întorc. Vin iar la party.

h: Data viitoare când ne luptăm, nu doar că am să *câștig*...

h: Am să-ți dau până *te omor*.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)