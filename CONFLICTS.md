# Árekstragreining

## Business Strategy Conflicts
1. **Dæmi #1**  
   - Átaksþáttur: [#2]  (https://github.com/Hvannberg/HBV301G-COS/issues/1)  
   Starfsmenn hafa áhyggjur af því að með því að fá matinn inn í deild og þar með raunvinnutími aukist, glatist félagsleg
   tengsl við aðra starfsmenn fyrirtækisins sem verða til í mötuneytinu sjálfu. Starfsmenn telja að það geti verið 
   erfitt að mæla árangurinn því starfsmenn stimpla sig ekki inn og út úr mat. 
   - Hagsmunaaðilar: Starfsmenn sem nota mötuneytið og Stjórnendur   
   - Lausn: Stjórnendur útskýra að auka megi félagsleg tengsl með öðrum hætti, t.d. heimsóknir eða viðburðir á milli deilda sem tæki þá minni tíma.   
   Stjórnendur munu  búast við því að raunvinnutími aukist yfir 12 mánuði en gerist ekki hratt. Stjórnendur munu  
   uppfæra orðalag viðskiptakröfu til að gera hana mælanlegri. Raunvinnutími er mældur með því að
   skoða gögn sem sýna viðveru starfsfólk á vinnustöð, t.d. með staðsetningu, gagnvirkni við verkfæri og/eða í dagbókum (fundir o.s.frv).

2. **Dæmi #2**  
   - Átaksþáttur: [#1] (https://github.com/Hvannberg/HBV301G-COS/issues/2) Kokkar segja að það verði óraunhæft að lækka kostnað vegna matarúrgangs um 40% 
   og biðja um nánari leiðbeiningar um hvernig þetta má vera. Þau benda einnig á að neytendur í mötuneytinu beri einnig ábyrgð á þessu og að auka þurfi vitundarvakningu 
   - Hagsmunaaðilar: Starfsmenn í framreiðslu í mötuneyti (kokkar) og Stjórnendur  
   - Lausn: Stjórnendur munu vinna nánar að leiðbeiningum til eldhúss um hvernig væri hægt að uppfylla kröfuna. Aðalsparnaðurinn mun fást 
   í fyrirsjáanleika matarskammta því starfsmenn panta matinn fyrirfram. Þau munu einnig
     setja af stað fræðslu fyrir mötuneytis neytendur. 

## Requirements Value Conflicts
3. **Dæmi #3**  
   - Átaksþáttur: Krafa [#20] (https://github.com/Hvannberg/HBV301G-COS/issues/20) Sendlum finnst óþarfi að kerfið sé aðgengilegt á nóttunni þegar engar sendingar fara fram. Einnig finnst
   þeim að starfsmenn geti pantað mat á milli 5 að morgni og miðnættis. Starfsmönnum sem vinna vaktavinnu vilja  geta pantað máltíðir á nóttunni þó svo að þeir fái ekki sendingar þá. Hér er því verið að 
   þjónusta vaktavinnustarfsmenn án viðbótarkostnaðar við að bjóða upp á sendingar á nóttunni. 
   - Hagsmunaaðilar: Starfsmenn sem panta mat úr mötuneyti (forgangsnotendur) og sendlar (ekki í forgangshópi)
   - Lausn: Þar sem Starfsmenn eru í forgangshópi notenda en ekki sendlar þá stendur krafan eins og hún er. Hins vegar ætti að gera orðalagið nákvæmara og leggja áherslu á að hægt sé að  
   panta 24/7 en afhendingar fari fram frá 5 til miðnættis. Einnig að viðhald á kerfinu fari fram á tímabilinu 12 og 5 á morgnana. Eins ef kerfið stöðvast þá er ekki þjónusta við það
   á þessum tíma. 

4. **Dæmi #4**  
   - Átaksþáttur: Í þessari kröfu er aðeins tekið fram fjölda samtímanotenda [#18] (https://github.com/Hvannberg/HBV301G-COS/issues/18) en ekkert talað um hve margar pantanir sendlar eiga 
   að afhenda í hverjum afhendingaglugga (sjá einnig viðskiptareglu [#3] (https://github.com/Hvannberg/HBV301G-COS/issues/3). Mötuneytisstarfsfólk bendir á að ekki sé tekið fram hversu mörgum máltíðum eldhúsið getur annað á kls. 
   - Hagsmunaaðilar: Sendlar, Mötuneytisstarfsfólk (sjá [Notendahópa SRS] (https://github.com/Hvannberg/HBV301G-COS/blob/main/SRS.md))  
   - Lausn: Þar sem mötuneytisstarfsfólk er í forgangshópi en sendlar ekki, þá verða sjónarmið mötuneytisstarfsfólk ofan á. Gætt verður að því að fjöldi sendla verði í takti við afköst eldhúss. 
   Sett verður inn ný krafa (takmörkun - constraints) sem segir til um að takmarka þurfi pantanir til afhendingar
   í takti við afköst eldhúss. Fjöldi leyfilegra pantana per afhendingaslot í kerfinu verður að endurspegla afköst eldhúss. 

## Requirements Substance Conflicts
5. **Dæmi #5**  
   - Átaksþáttur:   C1 [Oracle gagnagrunnur, #5](https://github.com/Hvannberg/HBV301G-COS/issues/5)  vs.  [Viðkvæm gögn skulu dulkóðuð með 256-bita dulritun #6](https://github.com/Hvannberg/HBV301G-COS/issues/6)
   Hér þarf að gæta þess að útgáfan af Oracle gagnagrunnskerfið styðji dulkóðun með 256-bita dulritun. 
   - Hagsmunaaðilar: Gagnagrunnsstjóri og persónuverndarstjóri þróunarteymisins   
   - Lausn: Á hönnunarstigi skal gæta þess að þessar tvær kröfur stangist ekki á þannig að hægt sé að uppfylla báðar. Einnig skal gera lista af þeim gagnagrunnskerfum öðrum en Oracle sem eru á markaðnum og tilvonandi   
   viðskiptavinir vilji mögulega nota. Setja þarf upp gátlista sem er notaður til að rýna útfærslu gagnagrunnsfyrirspurna m.t.t. þessara krafa.  

6. **Dæmi #6**  
   - Átaksþáttur:  SR1  [Notendaviðmót kerfisins er á vef, snjallsíma og kiosk #9](https://github.com/Hvannberg/HBV301G-COS/issues/9) | vs.   QR3 [Notendur skulu skrá sig inn á COS til að framkvæma allar aðgerðir nema til að skoða matseðla #19](https://github.com/Hvannberg/HBV301G-COS/issues/19)
   Er hægt að útfæra aðgang frá Kiosk með innskráningu í COS? eða rekast þessar kröfur á? Hvernig er farið með aðgang að COS frá ytra neti inn á innra net? 
   - Hagsmunaaðilar: Starfsmenn sem panta mat frá mötuneyti í gegnum Kiosk t.d. í mötuneyti og öryggisstjóri viðskiptavinar.   
   - Lausn:  Hér þarf að leyfa login á kiosk á auðveldan hátt t.d. með síma eða starfsmannakorti og gæta að því að notandi útskráist.  E.t.v. ætti að takmarka verkefni (tasks) á kiosk, t.d. matseðla eða athuga stöðu pantana.  

## Requirements Process Conflicts
7. **Dæmi #7**  
   - Átaksþáttur: Starfsfólk launadeildar eru fáliðuð og hafa ekki tíma til að taka þátt í kröfusöfnunarferlinu. Þau hafa mikla  
   þekkingu á launakerfinu sem tekur við færslum og eru því mikilvægur þátttakandi í ferlinu. 
   - Hagsmunaaðilar: Starfsfólk launadeildar, Viðskiptagreinandi, Stjórnendur  
   - Lausn:  Stjórnendur segja að ekki þurfi marga fundi með starfsfólki launadeildar. Fundirnir verða skipulagðir
   einni viku eftir mánaðarmót en á þeim tíma segir launadeild að það sé minnst álag. Fundir verða ekki á orlofstímum eða
   ef forföll eru í launadeildinni. 
   
8. **Dæmi #8**  
   - Átaksþáttur: Forritarar forrita samkvæmt virkniskröfunum sem viðskiptagreinandi hefur skrifað. Forriturum finnst þeir þurfi oft að breyta þeim en vilja  
   ekki viðhalda þeim. Vörustjóri og viðskiptagreinandi þurfa að rýna (review) breytingarnar.  Forriturum finnst það vera of mikil skriffinska og segja að enginn annar þurfi að vita af breytingunum
   - Hagsmunaaðilar: Forritarar, Vörustjóri, Viðskiptagreinandi
   - Lausn:  Stjórnendur skipar spretthóp um hvernig má styðja forritara í að viðhalda kröfum. Í hópnum eru forritari, prófari, viðskiptagreinandi og 
   vörustjóri. Hugmyndir stjórnenda eru betri verkfæri fyrir uppfærslu á kröfum, fræðsla frá prófurum um mikilvægi krafna sem inntak í prófanir og 
   aukið vægi á hlutverk vörustjóra sem tengiliður forritara og viðskiptagreinanda. 
