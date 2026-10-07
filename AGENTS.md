# Instruktioner till Codex

## Läs först

- `docs/PROJECT.md`
- `docs/EXPERIMENTS.md`
- `docs/DECISIONS.md`
- README för aktuellt experiment

## Arbetssätt

- Arbeta med små, reproducerbara experiment. Dokumentera mål, indata, kommandon, verktygsversioner, kontroller och resultat.
- Skilj verifierade fakta från användaruppgifter, hypoteser och öppna frågor.
- Börja med inventering av tidigare material innan nya data hämtas.
- Inventera angivna kataloger utan att flytta, ändra eller radera originalen. Arbeta på kopior vid bearbetning.
- Kontrollera befintliga filer och git-status innan ändringar. Bevara arbete som redan finns.
- Använd GDAL/OGR och scripts när det är lämpligt. Kontrollera vilka verktyg som faktiskt finns innan du väljer metod.
- Anta inte att en molnworkspace kan nå den lokala datorn, Trainz eller TransDEM. Redovisa vad som behöver köras lokalt.

## Geodata

- Ange källa, hämtningsdatum, villkor, geografisk täckning och relevanta dataår.
- Dokumentera horisontellt koordinatsystem, axelordning, enheter och höjdreferens. Gissa inte saknade referenssystem.
- Skilj kartans koordinatsystem från höjddatans vertikala referens.
- Dokumentera klippning, reprojektion, upplösning, NoData och resampling där det är relevant.
- Använd kända kontrollpunkter för att verifiera placering. En lyckad konvertering bevisar inte att geometrin ligger rätt.
- Kontrollera kompatibilitet mot de faktiska versionerna av Trainz och TransDEM före export.

## Lagring och verifiering

- Lägg rådata i `source-data/` och bearbetade filer i `generated/`. De katalogerna är ignorerade utom sina README-filer.
- Checka in scripts, metadata och små rapporter. Lägg inte in stora geodatafiler, installationspaket, kontouppgifter eller innehåll vars spridningsvillkor är oklara.
- Spara små avsiktliga testdata i ett experiments `fixtures/` och dokumentera ursprung och villkor.
- Kör kontroller som är relevanta för ändringen. Ange tydligt vad som verifierats automatiskt och vad som återstår i GUI eller på målsystemet.
- Uppdatera experimentloggen när ett försök ändrar status. Påstå inte att ett Trainz-resultat är verifierat om endast underlaget har kontrollerats.
