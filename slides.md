<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

## Upravljanje z verzijami

# git
<!-- .element: class="no-toc-progress" --> <!-- slide not in toc progress bar -->

##  in drugi primeri dobre prakse

pripravil [bojanra](https://github.com/bojanra) | 08.06.2022 | [online][1] | [src][2]

[1]: https://bojanra.github.io/Upravljanje-z-verzijami/
[2]: https://github.com/bojanra/Upravljanje-z-verzijami/

----  ----

## Zakaj upravljanje z verzijami?

* Scenarij:
  * Program/nastavitev dela
  * Opraviš "le eno spremembo"
  * Nekaj ne dela
  * Odpraviš spremembo
  * Še vedno ne dela - zakaj?

* Se vam je kdaj to zgodilo?

----

## Zakaj upravljanje z verzijami? (2)

* Scenarij:
  * Program/nastavitev je včeraj delovala
  * Že cel teden programiraš ali "pimpaš"
    * ne še čisto gotovo za produkcijo
  * Nujno je potrebno nekaj spremeniti v trenutni različici

* Se vam je kdaj to zgodilo?

----

## Zakaj upravljanje z verzijami? (3)

* Scenarij:
  * Več razvijalcev/uporabnikov dela na istem projektu
  * Sodelavec opravi nekaj sprememb
  * Tudi sam narediš nekaj popravkov
  * Datoteke si izmenjata
  * Na koncu nekaterih sprememb ni - zakaj?
  * Kdo je naredil kaj, kako se sinhronizirati

* Se vam je kdaj to zgodilo?

----  ----

## Klasični pristop

* naredimo "backup" delujoče verzije
* kopiramo direktorij ali naredimo **zip** arhiv

```
projekt_20211015.zip
projekt_20220315.zip
projekt_20220405.zip
projekt_20220521.zip
projekt_20220608.zip

```

* kako primerjati verzije med sabo?

----  ----

## Rešitev je **git**

* For working by yourself:
  * Gives you a “time machine” for going back to earlier versions
  * Gives you great support for different versions (standalone, web app, etc.) of the same basic project

* For working with others:
  * Greatly simplifies concurrent work, merging changes

----

## Namestitev

* Obstaja za različne platforme **Windows/Linux/Mac**
* Ukazna vsrtica
  * Git for Windows
* GUI orodja - https://git-scm.com/downloads/guis
  * GitHub Desktop
  * TortoiseGit
  * ...

----  ----

## Osnovni ukazi

* dodaj datoteko v **tracking**
```sh
git add primer.js
```

* dodaj verzijo v **arhiv**
```sh
git commit -a -m "Prestavi zanko v funkcijo"
```

* pregled zgodovine
```sh
git log
```

* pregled trenutnih sprememb
```sh
git status
```

----

## Še ne napredni ukazi

* pokaži spremembe od zadnje verzije
```sh
git diff
```

* primerjava med trenutno vezijo in verzijo `6e793406`
```sh
git diff 6e793406
```

* vrni se na verzijo `6e793406`
```sh
git checkout 6e793406
```

* vrni se na zadnjo različico
```sh
git checkout master
```

----

## in še bolj napredni ukazi

* začni z novim **branch**-om
```sh
git checkout -b novi_feature
```

* kloniraj obstoječi arhiv
```sh
git clone https://github.com/esp8266/Arduino
```

* prenesi spremembe iz kloniranega arhiva k sebi
```sh
git pull
```

* pošlji svoje spremembe v originalni arhiv
```sh
git push
```

----

## Redko uporabljeni,
### ampak neobhodno potrebni ukazi

* predstavimo se
```sh
git config --global user.name "Bojan Ramšak"
git config --global user.email bojan.ramsak@rtvslo.si
```

* ustvarimo nov **projekt**
```sh
git init
```

----  ----

# Dobra praksa

----

## Markdown

Pisanje je **Markdown** je preprosto

```markdown
## To je naslov

> "A framework for easily creating beautiful presentations using HTML."
>
> -- <cite>https://github.com/hakimel/reveal.js</cite>

* It's basically a website displayed in a browser
* Works better with Chrome than Firefox
* Markdown support -> easy editing:
  * Don't bother with xml syntax
  * Write slides in a markdown file
```

----

## To je naslov

> "A framework for easily creating beautiful presentations using HTML."
>
> -- <cite>https://github.com/hakimel/reveal.js</cite>

* It's basically a website displayed in a browser
* Works better with Chrome than Firefox
* Markdown support -> easy editing:
  * Don't bother with xml syntax
  * Write slides in a markdown file

----

## datoteka
# README.md

----

# git ni github

* https://github.com/
* https://bitbucket.org/


----

## Zanimiva orodja

* animacija
  * https://gource.io/
* orodje za prikaz razlik v direktorijih/datotekah
  * https://meldmerge.org/
* lastni "Github"
  * https://perlcodesample.sakura.ne.jp/gitprep/gitprep.cgi/kimoto/gitprep

----  ----

## Kaj drugi počnejo

* https://github.com/bbc/
* https://github.com/orgs/CasparCG/repositories
* https://github.com/IRT-Open-Source
* https://github.com/nrkno/Sofie-TV-automation
* https://github.com/drdk
* https://github.com/orgs/svt/repositories
* https://github.com/mediathekview
* https://github.com/ebu

