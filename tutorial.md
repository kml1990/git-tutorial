# Git tutorial

## **_git init_**

Zainitializuj repozytorium git.

## **_git add_**

Dodaj do stagu.

## **_git stash_**

Odkladanie zapisania kodu na pozniej (dodawanie go do temp folder)

### **_git stash pop_** - przywroc zapisany wczesniej kod i usuwa stos

### **_git stash apply_** - przywroc zapisany wczesniej kod i nie usuwa stos

### **_git stash push -m "dodatkowy kod"_** - dodaj dodatkowy kod do stos

### **_git stash list_** - pokaz liste stosow

### **_git stash clear_** - wyczysc stos

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

## **_git branch_**

### **_Master branch_**

Glowna galaz projektu wykorzystywana do publikacji najnowszej wersji projektu na serwerze produkcyjnym.
Master powinien zawsze zawierac stabilna wersje projektu. Mozliwosc wpowadzenia zmian powinna byc ograniczona.

### **_Dev branch_**

Galaz na ktorej znajduje sie wersja testowa projektu (alpha/beta), zwykle polaczona z serwerem testowym.

### **_Feature branch_**

Na tej galezi prowadzone sa pace nad nowymi funkcjami. Po ukonczeniu prac, zmiany trafiaja do branch dev.

### **_User branch_**

Galezie uzytkownikow sluza indywidualnej pracy czlonka zespolu nad zmianami. Ukonczone zmiany trafiaja na branch feature.

### **_Test/Bugfix branch_**

W szczegolnych przypadkach, konieczne jest szybkie wprowadzenie zmian. W tej sytuacji wykorzystywane sa branch'e typu bugix.
Przygotowane tutaj zmiany najczesciej trafiaja bezposrednio na branch dev.

### **_git branch_** - pokaz liste branchy

### **_git branch branchName_** - dodaj branch o nazwie branchName

### **_git checkout branchName_** - przejdz do branchu branchName

### **_git merge branchName_** - merge branchu z pozycji master

### **_git branch -b branchName_** - usun dany branch

---

## Komentarze ( 7 zasad )

---

- Podziel komentarz na tytul oraz tresc, oddzielajac je pustym wierszem
- Ogranicz tytul do 50 znakow
- Tytul rozpocznij Wielka litera
- Nie dodawaj kropki na koncu tytulu
- Uzywaj trybu rozkazujacego w tresci tytulu, np. Add e-mail field to login form zamiast New field in login form
- Ogranicz dlugosc wiersza tresci do 72 znakow
- Piszac tresc komentarza odpwiadaj na pytania co i dlaczego. Na pytanie jak mozna odpowiedziec przegladajac
  wprowadzone zmiany
