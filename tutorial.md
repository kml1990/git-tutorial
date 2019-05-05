# Git tutorial

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

## **_git revert_**

Revert to operacja polegajaca na odwroceniu zmian z wybranego commitu i zapisaniu
ich jako nowy commit. Polecnie moze byc uruchomione wylacznie na poziomie commitu.
Z pomoca git revert mozemy bezpiecznie przywracac zmiany ktore znajduja sie juz w
repozytorium publicznym.

## **_git reset_**

Przywraca zmiany w repozytorium do wskazanego punktu z histori zmian. Wazne: Nalezy
zachowac szczegolna ostroznosc podczas przywracania zmian z pomoca tego polecania.
Przywrocenie zmian oznacza modyfikacje historii comitow. Z tego powodu nie zaleca sie
stosowania tego polecania w przypadku commitow wyslanych do zdalnego repozytorium.

## **_git log_**

Pozwala podejzec historie commitow.

### **_git log --oneline_** pozwala podejzec historie repozytorium w przejzystej formie

### **_git log --author="Kamil"_** - pozwala podejzec historie repozytorium danego autora

### **_git log --oneline --author="Kamil"_** - laczenie

### **_git log --grep="view"_** - wyszukiwanie konkretnej frazy w komntarzach commitow

### **_git log --oneline -3_** - ile commitow chcemy zobaczyc

### **_git log --oneline -- index.html_** - sprawdzanie histori danego pliku

### **_git log --oneline --patch -- index.html_** - sprawdzanie co zostalo zmienione w danym pliku

### **_git log --oneline --summary -- index.html_** - sprawdzanie skroconej informacji o zmianach w pliku/ach

### **_git log --oneline --stat -- index.html_** - sprawdzanie statystyki zmian w pliku/ach.

### **_git shortlog_** - histria zmian z podzialem na uzytkownikow.

## Komentarze
