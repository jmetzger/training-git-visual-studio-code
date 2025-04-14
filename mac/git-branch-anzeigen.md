# Git branch anzeigen 

## Erklärung 

Auf dem Mac benutzt du wahrscheinlich `zsh` (seit macOS Catalina der Standard). Hier zeige ich dir, wie du den Prompt so anpassen kannst, dass du den aktuellen Git-Branch immer siehst.

---

### ✅ Schritt-für-Schritt-Anleitung

#### 1. Öffne deine `.zshrc` Datei:
```bash
nano ~/.zshrc
```

#### 2. Füge diesen Code ans Ende der Datei hinzu (oder passe deinen `PROMPT` an):

```zsh
autoload -Uz vcs_info

precmd() {
  vcs_info
}

zstyle ':vcs_info:git:*' formats '(%b)'

setopt prompt_subst
PROMPT='%F{cyan}%n@%m%f %F{yellow}%~%f %F{green}${vcs_info_msg_0_}%f
$ '
```

🧠 Erklärung:
- `%b` ist der aktuelle Branch.
- `${vcs_info_msg_0_}` enthält den Git-Branch, wenn du im Git-Verzeichnis bist.
- `%~` zeigt dein aktuelles Verzeichnis an.
- Farben: cyan = Benutzer@Host, gelb = Pfad, grün = Git-Branch

---

#### 3. Änderungen übernehmen:
```bash
source ~/.zshrc
```

---

### 🎁 Bonus: Noch schicker mit `Oh My Zsh`

Wenn du [Oh My Zsh](https://ohmyz.sh/) installiert hast, brauchst du nur ein Theme zu wählen, z. B. `agnoster` oder `robbyrussell`, die zeigen automatisch den Branch an:

```bash
ZSH_THEME="agnoster"
```

In deiner `~/.zshrc` Datei ändern und dann wieder `source ~/.zshrc`.
