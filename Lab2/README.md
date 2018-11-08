# Lab 2 - Provjera integriteta slike i kreiranje *Live* USB-a

U sklopu ove vježbe studenti će se upoznati sa pojmovima kao što integritet, te će koristiti besplatne alate kako bi provjerili i osigurali integritet podataka. Nakon toga ćete kreirati *Live* distribuciju Linuxa koju ćete pokrenuti sa USB-a.

## Vježba 1 - Provjera integriteta

Sa linka https://www.kali.org/downloads/ skinite **Kali Linux Light 64** verziju verziju Kali Linux distribucije. Da biste provjerili integritet skinute datoteke morate verificirati `sha256sum` koja vam je dana prilikom skidanja *image* datoteke (`.iso`).

Da biste to napravili, sa Microsoft-ove stranice skinite alat `fciv`: https://www.microsoft.com/en-us/download/details.aspx?id=11533 klikom na *Download*. Nakon što ste skinuli datoteku, raspakirajte je u Downloads mapi.

Otvorite *Command Prompt* te se pozicionirajte na *Downloads* mapu. Nakon toga pokrenite iz *Command Prompt-a* fciv alat kako bi provjerili integritet **Kali Linux Light 64** datoteke. Podudara li se `sha256sum` sa vrijednošću koja je dana na web-u?

## Vježba 2 - Kreiranje Live UBS distribucije Linuxa

Skinite alat Rufus sa sljedećeg linka: https://rufus.ie/en_IE.html
Nakon skidanja stavite USB u računalo, pod *Device* označite USB, dok pod *Boot selection* označite *Kali Linux Light 64* image datoteku (ekstenzija `.iso`) koju ste sačuvali (najvjerojatnije) u *Downloads* mapi. Ostala polja ostavite nepromijenjena.

Nakon što ste kreirali *Live* distribuciju pokušajte je pokrenuti sa računala tako da resetirate računalo, te u BIOS-u označite boot-anje sa USB-a kako bi se podigao operacijski sustav kojeg ste prethodno kreirali na USB-u