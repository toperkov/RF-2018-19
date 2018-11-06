# Lab 1 - Razumijevanje *hash* funkcija i hexadecimalne notacije

U sklopu ove vježbe student će se upoznati sa radom hash funkcija kao i sa hexadecimalnom reprezentacijom/notacijom.

## Vježba 1

Cilj ove vježbe je razumijeti da datoteke imaju jedinstvena zaglavlja na osnovu tipa datoteke. Pokazat ćemo kako datoteke ne trebaju imati ekstenziju za koje se trenutno prikazuju. Veoma bitno je kod računalne forenzike dtektirati datateke koje imaju primijenjenu ekstenziju, jer one mogu ukazivati na potencijalno skrivanje informacije.

- Skinite na vaše računalo te instalirajte Winhex program:
`http://www.winhex.com/winhex/hex-editor.html`

- Iz direktorija [Download](Download) sačuvajte 3 datoteke

- Svaku datoteku pojedinačno otvorite u `Winhex` editoru

- Korištenjem tablice potpisa datoteka pokušajte saznati o kojim tipovima datoteka se radi: http://en.wikipedia.org/wiki/List_of_file_signatures

# Vježba 2

Cilj ove vježbe je pokazati kako dvija datoteke kreirane u na različitim uređajima imaju iste hash otiske ukoliko je njihov sadržaj identičan. Također ćemo pokazati iako je sadržaj datoteke identičan (razlikuje se po kapitalizaciji) hash otisak će u tom slučaju biti isti.

- U Notepad-u kreirajte *text* dokument
- U dokument upišite vrijednost **test** te sačuvajte datoteku pod nazivom `test.txt`
- Kreirajte novi dokument te u njega upišite vrijednost **Test** te ga sačuvajte pod nazivom `test1.txt`
- U web pregledniku upišite: http://i-tools.org/hash
- Označite u padajućem izborniku MD5, SHA1 i SHA256 sa liste (držite pritisnutu tipku CTRL)
- Klikom na *Browse* označite datoteku test.txt koju ste prethodno sačuvali na svom računalu
- Kliknite na *generate* tipku na dnu forme
- Trebali biste dobiti ove rezultate:

```
--Test.txt--
MD5: 098f6bcd4621d373cade4e832627b4f6
SHA1: a94a8fe5ccb19ba61c4c0873d391e987982fbbd3
SHA256: 9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08

--#Test1.txt--
MD5: 0cbc6611f5540bd0809a388dc95a615b
SHA1: 640ab2bae07bedc4c163f679a746f7ab7fb5d1fa
SHA256: 532eaabd9574880dbf76b9b8cc00832c20a6ec113d682299550d7a6e0f345e25
```