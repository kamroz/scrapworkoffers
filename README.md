# scrapworkoffers
import urllib.request

def scraphtml (url):
    with urllib.request.urlopen(baseurl) as response:
        html = response.read()
        return html.decode('utf-8')

baseurl = "http://www.favore.pl/zlecenia,remonty-wykonczenia-wnetrz,woj-malopolskie-6,1015,0.html"
errand = str('<a href="/zlecenie/')

html = scraphtml(baseurl)

#wypisz na ekran pozycję pierwszej litery z łańcucha znaków ze zmiennej `errand`
#print(html.find(errand))

print("html rozmiar to: " + str(html.__len__()))
