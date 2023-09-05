# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Noroc!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah* ce bine a picat asta.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Știi, puștiule...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Mai precis, a picat exact pe amygdala cerebrală.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Îmi amintești de mine însumi când eram mai tânăr. Când eram și eu terorizat de animalul din capul meu.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Mă bucur tare mult că te pot ajuta, cum m-au ajutat și pe mine alții să omor dihania din mine.

```
publish("act3",["roofhunter",2]);
```

r: Scurtă întrebare: adevăr sau provo--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: CARE!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Okay.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. Vezi piscina aceea de-acolo de jos?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Aha .. De jos adică de *6 etaje* mai jos?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Da. Sari.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Poftim?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: A-nceput animalul să schelăie, așa-i?

```
publish("act3",["roofhunter",23]);
```

r: *Oh nuuuuuuu e periculos, să nu saaaaaari.*

```
publish("act3",["roofhunter",22]);
```

r: Exact ăsta e motivul pentru care avem nevoie de senzații tari! Party-uri! Carpe diem! Droguri, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Tre să-i arătăm animalului că nu dăm doi bani pe avertizările lui, pe  schelăiturile lui. Sari.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Da dar uneori.. totuși.. are sens frica...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Ah, scuze, să înțeleg că te-a convins propaganda Mindfulness că ți-e *bine* când ți-e rău?

```
publish("act3",["roofhunter",17]);
```

r: ^Rahații^ care conduc lumea asta ne dau ăstora celorlalți anxietate și depresie

```
publish("act3",["roofhunter",18]);
```

r: Și apoi ne explică la TED să "acceptăm" că suntem nenorociți și să permitem demonului sadic din noi să existe!

```
publish("act3",["roofhunter",6]);
```

r: Eu știu că și *tu* știi, puștiule, că animalul asta ne *rănește*. Ne *torturează*.

```
publish("act3",["roofhunter",19]);
```

r: Nu ne este prieten. E un animal sălbatic turbat care trebuie fie *tranchilizat*,

```
publish("act3",["roofhunter",20]);
```

r: fie *împușcat în cap, mortal*.

```
publish("act3",["roofhunter",27]);
```

r: Altfel îl lași să câștige.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Nu. Nu ai dreptate.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Nu am să-l las să câștige.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Așa da! Așa te vreau, știu că poți! Omoară-! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: nu nu nu nu nu nu

n: CAPITOLUL ASTA ARE DOUĂ POSIBILE FINALURI. UNUL DIN ELE E *FOARTE NASOL.*

b: NU NU NU NU NU NU NU NU NU NU NU NU NU NU

n: FĂ ALEGEREA CORECTĂ. PROTEJEAZĂ-ȚI OMUL.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: SUCCES

```
Game.clearText();
bb({ eyes:"start" });
```

[Poți SĂ MORI pe bune, acum, aici!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[E stupid și autodistructiv ce vrei să faci!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Demenții ăștia nu îți sunt cu adevărat prieteni!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: P--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: E--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: D--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Te-aș fi crezut poate, dacă nu mi-ai fi spus același lucru de un catralion de ori deja...

h: Ești lupul care a strigat "lupul!".

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Ai încercat și asta.

b: omule, te rog...

`hong({ eyes:"look_right" });`

h: *Regret nespus* că nu sunt de acord corporațiile farma ca eu să mă tratez singur.

h: Știi ce? *Toată* lumea încearcă să te facă să taci din gură, fiecare cum poate.

`hong({ body:"look_up", eyes:"look_up" });`

h: Unii oameni se aruncă în muncă.

`hong({ body:"look_down", eyes:"look_down" });`

h: Alții se aruncă în Facebook, sex sau droguri.

`hong({ body:"normal", eyes:"look_right" });`

h: Unii oameni se aruncă în alți oameni. 

`hong({ eyes:"angry" });`

h: Iar eu - eu am să mă arunc în această piscină.

[Ești beat și PISCINA E 6 ETAJE SUB NOI.](#act3_bad_1_harm)

[Astea sunt mulțumirile pe care le primesc?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Okay, recunosc. Am greșit.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Chiar dacă nimereși apa, tensiunea superficială din stratul de suprafață al apei îți poate rupe coastele, *cel puțin*!

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Am văzut o dată pe YouTube un rus care a făcut asta.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Pardon?! Poftim? *Mulțumiri?!*

`bb({ eyes:"angry" });`

b: Asta este motivul pentru care eu *exist*! Pentru că oamenii nu sunt în stare să aibă grijă de ei înșiși!

b: Toată viața n-am făcut decât să încerc să am grijă de tine și acum tu o să--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh Doamne Dumnezeule dacă nu e asta cea mai mare subestimare A SECOLULUI!

`hong({ body:"yell_2" });`

h: Da, animal împuțit nenorocit de mega ^căcat^! Absolut ai greșit! Și e puțin spus ai greșit!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Mai ai și alte remarci, Captain Obvious?

[Dar soluția nu este răzbunarea!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Dar de data asta *chiar* am dreptate!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Te-am rănit.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Trebuie să încerci să ai o relație mai sănătoasă cu propriile tale emoții, în loc să le înneci în--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Așa că te rog, pune sticla jos și hai să--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: te rog... nu...

h: Bara ta cu energie nu arată prea bine, lupoaică dragă.

h: În locul tău mi-aș alege cu foarte mare atenție următoarele cuvinte.

`bb({ eyes:"normal" });`

[Fie. Gata, nu te mai protejez.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Ha, am avut mereu dreptate.](#act3_bad_2_right)

[Îmi pare rău.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Așa că, hai, aruncă-te, sari. Nu-mi pasă.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Okay atunci. Până la fund.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NU! STAI! ASTA ERA PSIHOLOGIE INVERSĂ, TREBUIA SĂ FACI FIX *OPUSUL* A CEEA CE AM SPUS E--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Chiar* te pui tu pe tine însuți în pericol. Așa-zișii tăi prieteni *chiar* te folosesc. Iar *tu* îi folosești pe ei..

`bb({ eyes:"sad" });`

b: Așa că, te rog.. te rog, de ce nu mă crezi?!

h: Pentru că nici tu nu m-ai crezut niciodată pe *mine*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Altor lupi de pază le revin oameni care investesc timp în relație, îi duc la antrenament, *învață* să lucreze împreună,

b: În loc să își urască lupul pentru că acesta încearcă să îi protejeze! De ce nu poți fi și tu --

`bb({ eyes:"normal" });`

h: Răspuns greșit.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"Să nu îți fie frică decât de însăși frica."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Toți înțelepții de azi sunt de acord: emoțiile negative sunt *rele!*

`hong({ eyes:"less_angry" });`

h: Duh! De aia se și numesc *negative!*

b: omul meu... te rog...

`hong({ eyes:"normal" });`

h: Am zis acum mai demult că "tot ce vreau e să nu mai simt toată durerea asta!”

h: Mi s-a îndeplinit dorința. Nu mai simt, nici durere, nici frică, nici anxietate...

h: Nu mai simt absolut nimic.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Am fost obsedat de ideea că ceva ar putea să îți facă rău încât nu am realizat că *eu* îți făceam rău.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NU PE BUNE.

`hong({ body:"yell_1" });`

h: SERIOS?! Chiar ți-a luat atâta amar de vreme să îți dai seama?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Puteai să ne scutești pe amândoi de o grămadă de probleme. Cum de nu ai putut să înțelegi asta mai devreme?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...îți *pare rău*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: *pentru ce* îți pare rău?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Îmi pare rău că nu te-am protejat.](#act3_good_3_protector)

[Îmi pare rău că nu te-am respectat.](#act3_good_3_respect)

[Îmi pare rău.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Îmi pare rău că omul meu e oribil!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Îmi pare rău că nu te-am respectat.](#act3_good_3_respect)

[Îmi pare rău că te-am rănit.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Datoria mea este să te protejez de pericole *reale*, dar eu latru la mașini și la poștaș.

`bb({eyes:"sorry_up"});`

b: Latru la umbre. Latru prea mult.

`bb({eyes:"sorry"});`

b: Are sens atunci că vrei să îmi pui botniță.

`bb({eyes:"sorry_down"});`

b: Îmi pare rău.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: E responsabilitatea *mea* să te protejez și să te ascult, dar m-am comportat că și cum *tu* trebuie să asculți de mine orbește.

`bb({eyes:"sorry_up"});`

b: E o diferență între un protector și un paznic, iar eu am întrecut măsura.

`bb({eyes:"sorry_down"});`

b: Îmi pare rău.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Eram atât de obsedat de ideea de a te proteja cu orice preț încât nu am văzut că *eu* sunt cel care îți face rău.

`bb({eyes:"sorry_up"});`

b: Am fost un câine rău.

`bb({eyes:"sorry_down"});`

b: Îmi pare rău.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Era o idee stupidă oricum ai lua-o..

h: Nu am făcut asta decât să te enervez, și se pare că am reușit..

h: Hai să zicem că terminăm la egalitate, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Okay.

h: Okay.

n: *TIE*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Ei să nu-mi spui! După tot ce ți-a făcut animalul asta, acuma o să *renunți?*

r: Ce s-a-ntâmplat, puștiule? Ți s-a făcut *frică?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Da.

h2: Mi-e frică.

`publish('hong-next')`

h2: Și este absolut okay!

`publish('hong-next')`

h2: E okay să-ți fie frică.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: A-ncuiat cumva ușa?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
