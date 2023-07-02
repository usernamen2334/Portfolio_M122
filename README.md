# Input-Output_M122 (LA_122_1707)


## Einleitung:
In diesem Lernbericht möchte ich meine Erfahrungen und Erkenntnisse zum Thema Input-Output in PowerShell teilen. PowerShell ist eine leistungsstarke Skriptsprache von Microsoft, die speziell für die Verwaltung und Automatisierung von Windows-basierten Systemen entwickelt wurde. Die Verarbeitung von Ein- und Ausgaben ist ein entscheidender Aspekt bei der Entwicklung von PowerShell-Skripten.


## Verwendung
### Eingabe in PowerShell:
In PowerShell gibt es verschiedene Möglichkeiten, Eingaben zu verarbeiten:

Benutzereingaben über die Konsole: Mithilfe des Cmdlets "Read-Host" kann der Benutzer Texteingaben über die PowerShell-Konsole machen. Das Skript wartet, bis der Benutzer eine Eingabe macht, und speichert diese in einer Variablen.

```
$name = Read-Host "Geben Sie Ihren Namen ein"
Write-Host "Hallo, $name!"
```

Parameterübergabe beim Aufruf des Skripts: PowerShell-Skripte können auch mit Parametern aufgerufen werden. Diese Parameter können beim Ausführen des Skripts übergeben werden und dienen zur Konfiguration oder Personalisierung des Skripts.

```
param (
    [string]$name
)

Write-Host "Hallo, $name!"
```

### Ausgabe in PowerShell:
In PowerShell gibt es verschiedene Möglichkeiten, Ausgaben zu erzeugen:

Textausgabe auf der Konsole: Die Ausgabe von Text auf der Konsole erfolgt mithilfe des Cmdlets "Write-Host". Dieses Cmdlet gibt den angegebenen Text auf der Konsole aus.

```
Write-Host "Dies ist eine Textausgabe"

```
Ausgabe von Variablenwerten: PowerShell ermöglicht die direkte Ausgabe von Variablenwerten auf der Konsole, ohne explizit "Write-Host" verwenden zu müssen.


```
$name = "John Doe"
$name  # gibt den Wert der Variable $name aus

```

Ausgabe in Dateien: PowerShell bietet die Möglichkeit, Ergebnisse in Dateien zu schreiben. Dies kann mit dem Cmdlet "Out-File" erfolgen.
```
Get-Process | Out-File -FilePath "C:\Prozesse.txt"
```
## Reflexion:
Während meiner Auseinandersetzung mit Input-Output in PowerShell habe ich gelernt, wie vielseitig die Möglichkeiten zur Eingabe und Ausgabe in dieser Skriptsprache sind. Die Verarbeitung von Benutzereingaben mithilfe von "Read-Host" und das Arbeiten mit Parametern ermöglichen eine flexible Steuerung von Skripten. Die Ausgabe von Text und Variablenwerten auf der Konsole oder in Dateien ermöglicht eine effektive Kommunikation von Informationen. Ich habe auch festgestellt, dass PowerShell über eine umfangreiche Dokumentation und eine aktive Community verfügt, was die Entwicklung von Skripten erleichtert und bei auftretenden Fragen hilft.

Insgesamt hat mich die Arbeit mit Input-Output in PowerShell dazu befähigt, Skripte zu erstellen, die interaktiv mit dem Benutzer kommunizieren und Ergebnisse auf verschiedene Weisen ausgeben können. Ich bin motiviert, meine Kenntnisse in PowerShell weiter
