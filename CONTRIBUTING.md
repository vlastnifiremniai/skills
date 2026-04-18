# Přispívání

Tento repozitář je praktický katalog českých marketingových dovedností pro Claude Code, Codex a další AI nástroje. Přispívejte hlavně tím, co pomůže netechnickým uživatelům lépe zadávat opakované marketingové úkoly.

## Jak přidat novou dovednost

1. Vytvořte složku v kořeni repozitáře, například `vf-nazev-dovednosti/`.
2. Do složky přidejte `SKILL.md`.
3. Na začátek souboru vložte metadata:

```yaml
---
name: vf-nazev-dovednosti
description: Stručně popište, co dovednost dělá a kdy ji má agent použít.
---
```

4. Pište tělo dovednosti česky a prakticky.
5. Přidejte dovednost do tabulky v `README.md`.

## Styl psaní

- Pište přirozenou češtinou, ne doslovným překladem z angličtiny.
- Preferujte `výzva k akci` před `CTA`, `navazující e-mail` před `follow-up` a `cílová skupina` před `publikum`, pokud to zní přirozeněji.
- Udržujte dovednosti krátké. Ideálně do 300 slov.
- Nepřidávejte neověřená čísla, citace ani reference.

## Kontrola před odesláním

Spusťte nebo ručně ověřte:

```bash
rg --files
git status --short
```

Pokud máte dostupný validátor pro Agent Skills, použijte například:

```bash
skills-ref validate ./vf-copywriting
```

Zkontrolujte také, že název složky přesně odpovídá poli `name` v metadatech.

## Návrh změny

V návrhu změny stručně uveďte:

- jakou dovednost měníte nebo přidáváte;
- pro koho je užitečná;
- jak jste ověřili češtinu a strukturu `SKILL.md`.
