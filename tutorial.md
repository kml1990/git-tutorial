## **_git init_**

Zainitializuj repozytorium git.

## **_git add_**

Dodaj do stagu.

## **_git commit_**

Rejestrowanie zmian w repozytorium.

## **_git clean_**

Usuwa pliki, ktore nie zostaly dodane do indeksu gita.

## **_git reset_**

Przenosi pliki ze stage do working directory. Pelni odwrona
role niz git add.

## **_git rm / git mv_**

Usuwa / przenosi pliki w repozytorium. Dzialaja tak samo
jak rm i mv, i jednoczesnie dodaja zmiany na stage.

## **_git checkout_**

Checkout to peracja polegajaca na przesunieci wskaznika HEAD na wskazany commit.
W praktyce w katalogu roboczym zostaja wczytane pliki w wersji z wybrango commitu.
git checkout moze byc uzyte na poziomie commitu lub pliku. W tym drugim przypadku
zostanie wczytana wersja pliku z wubranego commitu (domyslnie z HEAD).

## **_git checkout (path)_**

Przywraca stan pliku z indeksu gita. W paktyce przywraca wpowadzon zmiany.
Moze byc wykorzystane tylko wtedy, gdy plikisntieje juz w indeksie.

## **_git log_**

Pozwala podejzec historie commitow.

### **_git log --oneline_** pozwala podejzec historie repozytorium w przejzystej formie
