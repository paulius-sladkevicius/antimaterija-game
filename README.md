# ANTIMATERIJA: DIDYSIS SUSIDŪRIMAS

Interaktyvi dvimatė dalelių simuliacija, rodanti materijos ir antimaterijos anihiliaciją.
Skirta vaikams, pritaikyta planšetei (horizontaliai, per visą ekraną), visa lietuvių kalba.

- 🔵 mėlynos dalelės – elektronai (materija, e⁻)
- 🔴 raudonos dalelės – pozitronai (antimaterija, e⁺)
- 🟡 geltoni spinduliai – gama fotonai (γ)

Pradiniame ekrane pasirenkama, kiek materijos ir antimaterijos paleisti: iš pradžių po 25, mygtukais „−“ ir „+“
galima keisti po 5, nuo 5 iki 100 (palaikius mygtuką skaičius keičiasi pats). Kai dalelių daugiau nei 50, jos
piešiamos mažesnės, kad tilptų ekrane.

Paspaudus **PRADĖTI EKSPERIMENTĄ**, elektronai ir pozitronai pradeda judėti ekrane.
Susilietus elektronui ir pozitronui įvyksta anihiliacija: blyksnis, garsas ir du fotonai,
išlekiantys tiksliai priešingomis kryptimis. Viršuje esantys skaitikliai rodo, kiek dalelių liko.

Pabaigoje parodoma, kiek įvyko anihiliacijų, kiek dalelių liko be poros (jei kiekiai buvo nelygūs) ir
„sąskaita“: viena sunaudota antimaterijos dalelė kainuoja 1000 eurų. **PAKARTOTI EKSPERIMENTĄ** grąžina į
pradinį ekraną, kur kiekius galima pakeisti.

## Kaip paleisti

Žaidimui nereikia nei diegimo, nei interneto – tai vienas `index.html` failas be išorinių priklausomybių.

- **Kompiuteryje ar planšetėje iš failo:** atidarykite `index.html` naršyklėje („Chrome“ arba „Samsung Internet“).
- **Iš interneto adreso** (pvz., „GitHub Pages“): atidarius pirmą kartą, žaidimas išsaugomas įrenginyje ir
  vėliau veikia be interneto. Naršyklės meniu pasirinkus „Įdiegti programą“ / „Pridėti prie pradžios ekrano“,
  jis atsidaro kaip atskira programa per visą ekraną, horizontaliai.

Vietinis serveris kūrimui: `python3 -m http.server` ir `http://localhost:8000`.

## Failai

| Failas | Paskirtis |
| --- | --- |
| `index.html` | Visas žaidimas: išdėstymas, stiliai, „Canvas“ simuliacija ir „Web Audio“ garsai |
| `sw.js` | Talpykla veikimui be interneto (pakeitus failus, padidinkite `CACHE` versiją) |
| `manifest.webmanifest`, `icon-*.png` | Diegimas į pradžios ekraną |

## Mokslinis tikslumas

Tai supaprastintas modelis. Elektrono ir pozitrono anihiliacija į du gama fotonus vaizduojama mažos energijos
atveju, kai dalelių sistemos bendras impulsas lygus nuliui – todėl fotonai išlekia priešingomis kryptimis.
Blyksnis, garsas ir matomi geltoni fotonai yra edukaciniai efektai, o ne tikros gama spinduliuotės vaizdas.
Kad eksperimentas visada pasibaigtų, ilgiau nevykstant reakcijoms priešingo krūvio dalelės pradeda švelniai
traukti viena kitą.
