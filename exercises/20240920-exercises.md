### Übungen während des Trainings 

```
## Tag 2 

## Übung 2.11 

1. neuen branch erstellen 

feature/<eurenname>2
feature/jochen2

2. todo.txt 

Ändern Zeile 1,5,12 

add + commit 

3. feature - branch pushen 

4. pull request 

------

## Übung 2.10 

1. neuen branch erstellen 

feature/<eurenname>1
feature/jochen1 

2. neue datei erstellen erstellen
jeder eine andere 
jochen8.txt 
add + commit 

3. feature - branch pushen 

4. pull request 





## Übung 2.9. 
 
 1.  workspace schliessen
 
 2. in git -> repo clonen 
 https://github.com/gitmeisterei/gruppe1.git




## Übung 2.8. 
0. you are in main 
1. LOKAL: neuen branch -> feature/4728
2. LOKAL wir machen eine ändern in README.md  Zeile 1,5,12
add  + commit 
---
3. ONLINE: im Branch main -> ändern wie in README.md 1,5,12
4 LOKAL: branch -> feature/4728 online push 
5. ONLINE: pull request erstellen  feature/4728 -> main 
---



## Übung 2.7. 

0. you are in main 
1. neuen branch -> feature/4727 
2. wie machen eine ändern in todo.txt 
3. push neuen branch nach github  .
ONLINE 4. machen einen pull request (und löschen den branch gleich nach dem Mergen -> Haken)
5. führen den pull-request (merge) 
--- 
6. aufräumen:
a. wechseln nach main
b. pull rebase 
c. feature/4727 löschen




2. Checkout new branch feature/4723
3. Change line1 in todo.txt 
4. git add -A; git commit -am "feature/4723 done"
5. Change to master 
6. Change line1 in todo.txt 
7. git add -A; git commit -am "change line1 in todo.txt in master" 
8. git merge feature/4723 



## Übung 2.6 

Hint: branch.<branchname>.rebase


0 . Voraussetzung: Gleicher Stand online wie offline 

1. LOKAL Wie machen eine Änderung lokal -> commit -> todo.txt 

2. REMOTE: Wie machen eine Änderung Online:   README.md  

3. Änderung von Online -> Remote abholen 
pull --rebase 



## Übung 2.5. - 

1. LOKAL: änderung lokal -> commit 
README.md 

2. REMOTE jemand eine änderung online  
todo.txt 

3. LOKAL: push  





## Übung 2.4. _ Änderungen abholen 

1. Online Änderung machen 
2. commit online und lokal vergleichen
3. Änderungen abholen -> pull 



## Übung 2.3. -> Schattenbranch -> wo ? 

auf der kommandozeile 

cd .git
ls -la
cd refs
cd remotes
cd origin 
ls -la
cat main
cd ../../../..





## Übung 2.2 (vscode) 

git remote  set-url  origin https://github.com/gitmeisterei/trainerseins.git




## Übung 2.1 (vscode) 

1. Suchen uns altes commit (git graph)
2. Und machen eine revert
3. und schauen das revert an 



## Tag 1

## Übung 1.11 (vscode) 

1. Erstellen neuen branch
feature/4721 

2. Erstellen eine neue datei : datei1
add + commit

3. Erstellen eine neue datei : datei2
add + commit

3. Erstellen eine neue datei : datei3
add + commit

4.  in main wechseln 

5. commit mit datei3 cherry-picken 

6. branch feature/4721 löschen 





## Übung 1.10 (vscode) 

1. ordner tmp erstellen 
2. in dem ordner eine datei test.exe anlegen und add + commit 


3 .gitignore auf tmp ordner setzen
im Wurzelverzeichnis 
.gitignore 
/tmp/*.exe 
clear
add + commit 

4. änderung in test.exe 
5. eine neue datei start.exe 

6. auf der kommandozeile 

git rm --cached tmp/test.exe

7. bitte testen

-> änderung test.exe und start.exe
erscheinen dateien im Index -> git -> source control 




## Übung 1.7. (vs code) 

0. Ausgangspunkt: main 

1. Wir erstellen einen neuen Branch und checken aus:
feature/4713 

2. einige Änderungen 

todo.txt:
Zeile 1
Zeile 3
Zeile 5 

README.md 
Zeile 5  (wenn nicht da, hinzufügen) 

ad + commit 

3. wir wechseln in main 

4. Änderungen folgenden Dateien 

todo.txt 
Zeile 1
Zeile 3 
 
README.md
Zeile 1
Zeile 5 

add + commit 

5. merge von feature/4713 nach main (current branch)

# Übung 1.6 (vs code) 

=. Ausgangspunkt im main

1. branch erstellen und auschecken  
feature/4712

2. in diesem eine branch feature/4712 eine Änderung machen
neue datei z.B. 
jochen2.txt 
add + commit

3. Wieder in den main branch zurückwechseln    
    
4. git merge --no-ff feature/4712 (bitte haken nicht rausnehmen) 

 



# Übung 1.5. (vs code) 

git graph 
über feature/4711 gehen 
rechts maustaste
merge into current branch 



# Übung 1.4 (vs code)

1. branch erstellen und auschecken  
feature/4711 

2, Forschung:
 Was passiert unter der Haube 

3.  Verzeichnis anschauen
ls -la .git
cat .git/HEAD
git checkout main



4. in diesem eine branch feature/4711 eine Änderung machen
neue datei z.B. 
jochen.txt 

 
 5. Wieder in den main branch zurückwechseln    
    
6. 

cat .git/refs/heads/main
cat .git/refs/heads/feature/4711



## Übung 1.3
stand davor:
git reflog 
git reset --hard d00c


## Übung 1.2.

1. änderung in der todo.txt machen und committed

2. änderung mit einem reset (--hard, --mixed, -- soft) 



## Übung 1.1 

1. auf der Kommandozeile Ordner mit versteckten Dateien anzeigen
ls -la
cd .git
ls -la
cd objects

git cat-file -p

```
