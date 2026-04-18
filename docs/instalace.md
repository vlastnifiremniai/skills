# Instalace dovedností

Tento repozitář používá jednoduchý formát Agent Skills. Každá dovednost je samostatná složka v kořeni repozitáře a obsahuje soubor `SKILL.md`.

## Doporučená instalace

Po publikování repozitáře použijte:

```bash
npx skills add vlastnifiremniai/skills
```

Instalace jen vybraných dovedností:

```bash
npx skills add vlastnifiremniai/skills --skill vf-konverzni-strategie vf-copywriting vf-seo-audit
```

Instalace pro konkrétní agenty:

```bash
npx skills add vlastnifiremniai/skills --agent claude-code codex
```

Výpis dostupných dovedností:

```bash
npx skills add vlastnifiremniai/skills --list
```

## Claude Code

Pokud váš nástroj umí pracovat s dovednostmi ve formátu `SKILL.md`, zkopírujte vybrané složky do projektu:

```bash
mkdir -p .agents/skills
cp -r vf-konverzni-strategie vf-copywriting vf-seo-audit .agents/skills/
```

Některá nastavení Claude Code nebo podobné nástroje mohou očekávat i složku `.claude/skills/`:

```bash
mkdir -p .claude/skills
cp -r vf-konverzni-strategie vf-copywriting vf-seo-audit .claude/skills/
```

Claude Code má také subagenty ve složce `.claude/agents/`. Je to podobný, ale samostatný mechanismus. Tento repozitář používá dovednosti se soubory `SKILL.md`.

## Codex

Pro lokální Codex zkopírujte vybrané dovednosti do uživatelské složky:

```bash
mkdir -p ~/.codex/skills
cp -r vf-konverzni-strategie vf-copywriting vf-seo-audit ~/.codex/skills/
```

Pro projektové použití je praktičtější uložit dovednosti do `.agents/skills/`, aby byly dostupné i dalším AI nástrojům v repozitáři.

## Multi-agent nástroje

Pokud používáte SkillKit:

```bash
npx skillkit install vlastnifiremniai/skills
```

Vybrané dovednosti:

```bash
npx skillkit install vlastnifiremniai/skills --skill vf-konverzni-strategie vf-copywriting vf-seo-audit
```

## Jak začít

1. Nainstalujte `vf-marketingovy-kontext`.
2. Požádejte agenta: `Vytvoř marketingový kontext pro naši firmu.`
3. Dovednost vytvoří `.agents/marketingovy-kontext.md`, pokud ještě neexistuje.
4. Potom používejte další dovednosti, například `vf-konverzni-strategie`, `vf-copywriting` nebo `vf-seo-audit`.
