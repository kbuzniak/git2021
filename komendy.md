#Polecenia w terminalu - operacje na koncie lokalnym gita
git init - tworzy nowe repozytorium w projekcie
git clone - pobieramy repozytorium zdalne https://github.com/kbuzniak/git2021.git
git status - sprawdzamy stan repozytorium
git add - dodawanie pliku do śledzenia
git add nazwa_pliku
git add nazwa_folderu
git add . - wszystkie pliki

git rm --cached README - usumięcie pliku README ze śledzenia
git reset - usuwa wszystkie pliki ze śledzenia - sprawdzić: git status

git commit - wysłanie zmiany do lokalnego repozytorium  
 git commit -a - dodaje i wysyła, lepiej zrobić git add i git commit oddzielnie
git commit -m "komentarz"
git restore nr_git_log - przywraca konkretny plik do wersji z repozytorium, ale lepiej zrobić commit  
git log - pokazuje wszystkie commit-y wykonane w repozytorium
git revert nr_git_log - wycofanie wybranego commit-a
git show nr_git_log - wyświetla zmiany w konkretnym commit-cie, bez nr_git_log wyświetli ostatni commit

git commit --amend "zmiana" - zmiana komentarza

#Polecenia w terminalu - operacje na koncie GitHub
git clone ścieżka_z_GitHub - pobiera pliki z repozytorium GitHub-a

git status
git add .
git push - publikuje lokalne zmiany zmiany w repozytorium GitHub-a
git pull - pobiera zmiany z repozytorium zdalnego

#branche - gałęzie
git checkout -b nazwa_brancha - utworzenie nowej gałęzi i przejście na nią
git checkout -b feature/1-header_do_pliku_index
git push --set-upstream origin feature/1-header_do_pliku_index - tworzenie gałęzi na GitHubie
