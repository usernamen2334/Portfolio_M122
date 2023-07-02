# Input-Output_M122 (LA_122_1707)


## Einleitung:
In diesem Lernbericht möchte ich meine Erfahrungen und Erkenntnisse zum Thema Input-Output in PowerShell teilen. PowerShell ist eine leistungsstarke Skriptsprache von Microsoft, die speziell für die Verwaltung und Automatisierung von Windows-basierten Systemen entwickelt wurde. Die Verarbeitung von Ein- und Ausgaben ist ein entscheidender Aspekt bei der Entwicklung von PowerShell-Skripten.


## Verwendung
Eingabe in PowerShell:
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
