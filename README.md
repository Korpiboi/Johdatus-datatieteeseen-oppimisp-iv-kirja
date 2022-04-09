# Johdatus-datatieteeseen-oppimispaivakirja
JodaTuni :D Päiväkirja

1.	Kerro osallistuitko viikon opetukseen ja kuvaa päiväkirjan laatimisessa käyttämäsi aineisto.
2.	Tiivistä jokaisen luentoviikon keskeiset asiat tekstiksi.
3.	Kirjaa lisäksi ylös viisi oivallusta tai tärkeintä oppimaasi asiaa erilliseksi listaksi.
4.	Listaa yhdestä kolmeen kehityskohdetta tai flippausvinkkiä luentoviikolle.
5.	Kokoa noin kymmenen koodirivin demo viikon aikana oppimastasi.

Viikko 1:

1)
Ensimmäiselle luennolle en päässyt paikanpäälle. Sen sijasta katsoin Panoptosta kevään 2021 aloitusluennon. Katsoin myös vanhan koodiklinikan panoptosta.

2)
Ensimmäisellä luennolla kerrottiin aluksi kurssin historiasta ja tarkoituksesta. Seuraavaksi esiteltiin kurssin suoritusvaatimukset, eli harjoitustyö ja luentopäiväkirja. Luennolla käytiin läpi datatieteen perusteita, kuten mitä se edes tarkoittaa.
Luennolla esiteltiin kurssilla opeteltavia python pohjaisia sovelluksia, kuten Jupyter, ja Pandas. Meille näytettiin myös mitä kannattaa ladata omalle koneelle, että tarvittavat sovellukset saadaan toimimaan. Itse latasin Anaconda Navigatorin luennon aikana. Kurssilla kuulemma koodataan ja sen osaaminen hyvin auttaa paljon. Toivon että muistan vielä jotain Johdatuksesta ohjelmointiin, jonka kävin viisi vuotta sitten.
Perehdyimme siihen mitä tarkoittaa olla ”data scientist”, sekä datatieteen eroihin ja samanlaisuuksiin perinteisen tilastotieteen kanssa. Katsoimme useita kuvia, jotka havainnollistivat datatiedettä eri näkökulmista. 
Perjantaina katsoin vanhan koodiklinikka demon. Kirjoittelin itse Jupyterilla mukana ja testailin asioita. Opin paljon ja sovellus vaikutti hyödylliseltä ja helpolta käyttää. Opetus meni nopeasti tosin, minkä takia tallenne oli minulle hyvä.

3)

Viisi oivallusta luennolta:
1. Koodaus on kurssilla huomattavasti tärkeämpää kuin oletin.
2. Datatiede eroaa tilastotieteestä enemmän kuin kuvittelin. Luulin niiden olevan    lähes sama asia.
3. Kurssi suoritetaan pelkästään harjoitustyöllä ja oppimispäiväkirjalla. Ei tenttiä.
4. Jupyter vaikuttaa erittäin monikäyttöiseltä ja hyödyllisestä 
5. CSV tiedon muokkaaminen ja esittäminen on helppoa Jupyterilla

4)
Katsoin Panoptosta vanhan koodi demon. Siinä mentiin hyvin nopeasti eteenpäin omasta mielestä, mikä hankaloittaa oppimista, jos ei katso tallenteita. Hitaampi eteneminen auttaisi siis oppimista.
5)
import pandas as pd
import matplotlib.pyplot as plt
from matplotlib import style
style.use('ggplot')

# Käytettävien kirjastojen importtaamista. Kirjastoilla plotataan (matplotlib) ja luetaan/muokataan dataa (pandas)
sivu = ’https://jokudatatiedosto.csv’
originaali = pd.read_csv(sivu)
tiedosto = originaali.copy()
print('List of attributes:', tiedosto.columns.values.tolist())
# Lukee halutun nettisivun csv muotoista tietoa ja tallentaa sen muuttujaan. Printtaa listan kolumnien attribuuteista

tiedosto_plot = pd.DataFrame([[numero1, numero2, numero3, numero4]])
tiedosto _plot.columns = ['Kategoria1', ' Kategoria2', ' Kategoria3', ' Kategoria4']
tiedosto _plot.plot.bar(figsize=(10,7))
plt.legend(loc=2)
plt.ylabel('Sum $')
plt.show()
# Plottaa mitkä vaan numerot siististi.
