# Pošta – vydání

Instalačky osobního mail klienta **Pošta** pro macOS a Windows.
Zdrojový kód je v soukromém repozitáři, tady jsou jen hotové verze.

## Stažení

Nejnovější verze je v sekci
[**Releases**](https://github.com/Bartyx/posta-releases/releases/latest):

- **macOS:** soubor `.dmg` (Intel i Apple Silicon),
- **Windows:** soubor končící `-setup.exe`.

Nainstalovaná Pošta si nové verze najde a nainstaluje sama.

## První spuštění

Aplikace není podepsaná certifikátem Apple ani Microsoftu, takže ji systém
při prvním spuštění zablokuje:

- **macOS:** přetáhni Poštu do Aplikací a otevři ji. Když se objeví hláška,
  že ji nelze ověřit, jdi do *Nastavení systému → Soukromí a zabezpečení*
  a klikni na *Přesto otevřít*. Kdyby macOS hlásil, že je aplikace
  „poškozená“, spusť v Terminálu `xattr -cr /Applications/Pošta.app`.
- **Windows:** v okně SmartScreen klikni na *Další informace → Přesto spustit*.

## Automatické aktualizace

Pošta stahuje soubor `latest.json` z nejnovějšího vydání v tomto
repozitáři. Každá aktualizace je podepsaná soukromým klíčem autora a
aplikace nainstaluje jen aktualizaci s platným podpisem.

Soubory v tomto repozitáři nahrává automaticky GitHub Actions, ručně se
sem nic nepřidává.
