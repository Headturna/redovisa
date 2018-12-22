---
---
Rapport kmom05
=========================

Utvärdera webbplatsers laddningstid.
-----------------------

I rapporten skall tre webbplatsers laddnigstid och prestanda mätas och analyseras.


###Urval


De tre webbsplatser som valdes är inom samma kategori; online video-streaming hemsidor.
Det är viktigt för dessa hemsidor att ha en snabb laddningstid och bra generell prestanda, eftersom att webbplatserna är främst gjorda för underhållning.

Det skall vara lätt att hitta på hemsian, och nya videos och flikar skall laddas in snabbt och smidigt, även på lite sämre bredbandshastigheter.

Av dessa tre hemsidor är YouTube och Twitch de mest "förfinade" och genomtänkta. Den sista är en mindre optimerad hemsida, Mixer. Den är med för jämförelsens skull.

Dessa hemsidor valdes för att de är väldigt populära, vilket innebär att de får många besökare. Därmed är det extra viktigt att de har en hög standard när det gäller laddnigstid och prestanda.

* <a href="https://www.youtube.com" target="_blank">YouTube</a>
* <a href="https://www.twitch.tv" target="_blank">Twitch</a>
* <a href="https://www.mixer.com" target="_blank">Mixer</a>

###Metod


Hemsidornas laddningstid, storlek och antal element som laddas dokumenteras.
Medelvärdet av dessa tre värden beräknas utifrån att tre tester görs för varje hemsida. Testerna består av att ladda om hemsidan så att nya mätvärden visas.
De verktyg som användes är webbläsarens egna devtools. Här användes främst data från "Networks" fliken.
Google Pagespeed användes för att hämta ett betyg för varje webbplats, både för mobil och dator versionen, enligt Googles egna bedömningstekniker.
Alla värden sparades i ett Google Kalkylark och för det så användes Google Sheets.

* <a href="https://developers.google.com/speed/pagespeed/insights/" target="_blank">Google Pagespeed</a>
* <a href="https://docs.google.com/spreadsheets/d/1DGs4wKKgjY_qgtLhpzMej8M4Q_k_jK_CjBrVANcv8-s/edit?usp=sharing" target="_blank">Google Kalkylark med data</a>

###Resultat


Youtube:

[FIGURE src=image/Youtube.png?w=500]

YouTube fick ett betyg av 47 för sin mobil version, samt ett betyg av 83 för sin dator version. Med devtools får hemsidan en medel-laddningstid på 1.53 sekunder, samt 63 resurser laddade och en total storlek på 139 kb.

Twitch:

[FIGURE src=image/Twitch.png?w=500]

Twitch fick ett betyg av 43 för sin mobil version, samt ett betyg av 87 för sin dator version. Med devtools får hemsidan en medel-laddningstid på 0.85 sekunder, samt 128 resurser laddade och en total storlek på 2233 kb (detta på grund av den aktiva video-streamen på index sidan).

Mixer:

[FIGURE src=image/Mixer.png?w=500]

Mixer fick ett betyg av 27 för sin mobil version, samt ett betyg av 85 för sin dator version. Med devtools får hemsidan en medel-laddningstid på 1.07 sekunder, samt 133 resurser laddade och en total storlek på 167 kb.

###Analys


YouTube:

Laddningstiden är snabb och ordningen av elementen som laddas in känns rätt. På sidan som laddas in finns det inte så många stora element som kräver längre laddningstider.

Twitch:

Laddningstiden är relativt bra men sämre än YouTube. På Twitch finns det betydligt många fler element som laddas in. På index sidan finns det en aktiv video-stream som laddas in samt många mindre bilder och element. Dessa element renderas inte samtidigt och det ger en känsla av att hemsidan är mindre optimerad. När man klickar sig in på en individuell stream så är laddningstiden snabbare eftersom det är mindre element som laddas in.

Mixer:

Mixer är relativt bra optimerad. På index sidan så laddas många element in, men inte lika många som på twitch. Element laddas in, mer eller mindre, samtidigt och individuella streams laddar in snabbt.

Samlade intryck:

Hemsidorna laddar generellt snabbt och är optimerade för videouppspelning och bilder. Laddningen av dessa ska ske snabbt och skall prioriteras. Det bästa enligt Google Pagespeeds verkar vara att använda rätt och moderna bild- och videoformat samt att bilder ska vara i rätt storlek. Även att minifiera css, javascript och annan kod.
Dessa tre hemsidor verkar, som sett via devtools, ladda in mycket element i förväg innan en stor rendering sker. Samt att de fortsätter ladda in element i bakgrunden så att hemsidan bara ger ett intryck av att vara färdigladdad.
Generellt så kan de minska antalet element och storleken på bilder, samt minifiera css och javascript. Hemsidor med live video-streaming på index sidan kan också minska storleken på videon.

Rangordning för webbplatserna:

Hemsidorna har rangordnats enligt datan som samlats in.

1. Youtube
2. Mixer
3. Twitch

Denna rangordningen har bestämts för att YouTube är den hemsida som laddar snabbast och använder minst resurser. När hemsidan laddas in så renderas allting samtidigt.
Mixer laddar, precis som YouTube, snabbt och det som skall renderas visas samtidigt.
Twitch hamnar sist eftersom att laddningstiderna är inte de bästa och olika element laddar in snabbare än andra.
Innan alla mätningar skedde så antogs det att Mixer skulle vara den sämst optimerade hemsidan, men detta antagande var fel.

Gräns för absolut laddningstid:

Enligt min åsikt så ska det inte ta mer än en och en halv sekund för en hemsida att laddas in, och inte mer än två sekunder för den att rendera allting viktigt och vara färdigladdad.

###Referenser

Inga referenser användes.

###Övrigt


Suraj Sharma.
