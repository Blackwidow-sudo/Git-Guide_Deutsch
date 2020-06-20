# GitHub

#### Repository
Ein Repository ist eine Bibliothek von Quellcode Dokumenten (nicht zwangsläufig Quellcode).
Man muss unterscheiden zwischen einem lokalen Repository und einem Remote-Repository.
Mehr dazu im Abschnitt 'Git'.

#### Master
Erstellt man ein neues Repository ist dieses die 'Master'-Version.

#### Branch (Zweig)
Wenn man beispielsweise ein neues Feature für ein Projekt (zB eine App) schreiben will, 
erstellt man einen neuen 'Branch' von 'Master'. In diesem Branch schreibt
man dann seinen neuen Code, der das Feature bilden wird. Wenn das Feature fertig gestellt, getestet und bereit für
die Implementierung in das Projekt ist, wird der Branch mit Master verschmolzen (merge).

#### Merge
Merge bedeutet soviel wie verschmelzen, fusionieren oder vereinigen.
Beispiel:
  - Erstelle 'Feature' branch von 'Master'
  - Commit Changes
  - Merge 'Feature' branch in 'Master' hinein

#### Pull Request (Import Anfrage)
Wenn man sich beispielsweise an einem OpenSource-Projekt beteiligt für das man ein neues Feature schreibt,
muss man vor dem 'Merge' eine 'Pull Request' an den Besitzer des Repository's stellen. Der Besitzer des Repository's
wird dann benachrichtigt über deine Anfrage und kann sich den angebotenen Code anschauen und ihn mit dir besprechen.
Ist der Besitzer zufrieden und gibt sein OK, wird dein 'Branch' in 'Master' gemerged.

# Git

#### Um einen Arbeitsordner zu initialisieren:

```git init```

#### Zur Statusabfrage:

```git status```


### Ein lokales Repository besteht aus 3 Instanzen die von Git verwaltet werden

1. Der Arbeitsordner (also der, den man sieht und in dem man neue Dokumente anlegt)
2. Der Index, welcher als Zwischenstufe agiert (Stage)
3. Der HEAD, der auf deinen letzen Commit zeigt.

#### Um Dateien auf den Index zu setzen (Stage):
  - ```git add .``` Um alle Dateien im Arbeitsordner zu stagen
  - ```git add DATEI``` Um eine DATEI zur Stage hinzuzufügen

#### Um die Dateien vom Index zum HEAD zu commiten:
```git commit -m 'Beschreibung'```

### Arbeiten mit einem Remote-Repository (zB auf GitHub)

Die Änderungen sind jetzt im HEAD deines lokalen Repositories.
Um die Änderungen an dein entferntes Repository zu senden:

```git push origin master```

Master lässt sich auch durch einen beliebigen anderen Branch ersetzen.

Wenn man sein lokales Repository aber mit einem leeren Remote-Repository auf GitHub verbinden möchte


#### Git Commands

```git clone``` Bring a Repository that is hosted on GitHub into a Folder on your local Machine.

```git add``` Track your Files and Changes in Git

```git commit``` Save your Files in Git

```git push``` Upload Git-Commits to a remote Repo, like GitHub

```git pull``` Download Changes from the remote Repo to your local machine, the opposite of ```push```
