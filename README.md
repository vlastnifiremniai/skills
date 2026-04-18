# České AI dovednosti pro marketing, Claude Code a Codex

České marketingové dovednosti pro AI nástroje jako Claude Code, OpenAI Codex, Cursor nebo Windsurf. Repozitář `vlastnifiremniai/skills` pomáhá lidem bez technického zázemí zadávat opakované marketingové úkoly, aniž by pokaždé psali zadání od nuly.

## Co je v repozitáři

Každá dovednost je samostatná složka v kořeni repozitáře:

```text
vf-copywriting/
└── SKILL.md
```

Soubor `SKILL.md` říká, kdy má AI nástroj dovednost použít, na co se má zeptat a v jaké podobě má vrátit výstup.

## Dostupné dovednosti

| Dovednost | K čemu slouží |
| --- | --- |
| `vf-marketingovy-kontext` | Vytvoří `.agents/marketingovy-kontext.md` s informacemi o firmě, produktu, zákaznících, nabídce a tónu komunikace. |
| `vf-copywriting` | Píše a přepisuje české prodejní texty pro weby, landing page, nabídky, produktové stránky a kampaně. |
| `vf-konverzni-strategie` | Pomáhá zjistit, proč nabídka, stránka, e-mail nebo kampaň nekonvertuje, a navrhuje konkrétní úpravy nabídky, sdělení, důvěryhodnosti a výzvy k akci. |
| `vf-editace-textu` | Zkracuje, zpřesňuje a zlidšťuje hotové texty. |
| `vf-zakaznicky-vyzkum` | Připravuje otázky pro zákaznické rozhovory, dotazníky a shrnutí odpovědí. |
| `vf-obsahova-strategie` | Navrhuje obsahové pilíře, témata, formáty a publikační plán. |
| `vf-socialni-obsah` | Připravuje příspěvky pro LinkedIn, Facebook, Instagram, X a další sociální sítě. |
| `vf-emailova-sekvence` | Vytváří uvítací, prodejní, vzdělávací a navazující e-mailové série. |
| `vf-cold-email` | Píše krátké B2B obchodní oslovení a navazující e-maily. |
| `vf-seo-audit` | Kontroluje stránku, článek nebo webový obsah z pohledu SEO. |
| `vf-optimalizace-landing-page` | Zlepšuje strukturu, argumentaci a konverzní prvky landing page. |

## Rychlá instalace

Nainstalujte celý katalog:

```bash
npx skills add vlastnifiremniai/skills
```

Nainstalujte jen vybrané dovednosti:

```bash
npx skills add vlastnifiremniai/skills --skill vf-konverzni-strategie vf-copywriting vf-seo-audit
```

Instalace pro konkrétní agenty:

```bash
npx skills add vlastnifiremniai/skills --agent claude-code codex
```

Další možnosti jsou v [návodu k instalaci](docs/instalace.md).

## Doporučený začátek

Nejdřív použijte `vf-marketingovy-kontext`:

```text
Vytvoř marketingový kontext pro naši firmu.
```

Tato dovednost vytvoří `.agents/marketingovy-kontext.md`. Ostatní dovednosti z něj čtou informace o firmě, nabídce, cílové skupině a tónu komunikace, takže se AI nástroj nemusí ptát pořád na stejné věci.

## Příklady použití

```text
Použij vf-copywriting a napiš lepší text pro landing page našeho účetního servisu.
```

```text
Použij vf-konverzni-strategie a řekni, proč tahle nabídka negeneruje poptávky.
```

```text
Použij vf-emailova-sekvence a připrav pět e-mailů pro nové zákazníky po registraci.
```

```text
Použij vf-seo-audit a zkontroluj tento článek z pohledu SEO.
```

```text
Použij vf-socialni-obsah a připrav tři LinkedIn příspěvky z tohoto článku.
```

## Pro koho to je

- malé a střední firmy, které chtějí používat AI v marketingu;
- freelanceři a konzultanti pracující v češtině;
- týmy používající Claude Code, Codex nebo jiné AI nástroje;
- lidé, kteří chtějí opakovatelné marketingové postupy místo jednorázových zadání.

## Doporučená témata pro GitHub

Pro lepší dohledatelnost nastavte v sekci About na GitHubu tato témata:

```text
agent-skills
ai-agents
claude-code
codex
cursor
marketing
marketing-skills
copywriting
seo
czech
czech-language
vlastni-firemni-ai
```

Krátký popis repozitáře do sekce About:

```text
Czech marketing Agent Skills for Claude Code, Codex and AI agents: copywriting, SEO, landing pages, e-mail sequences and customer research.
```

## English Summary

This repository contains Czech marketing Agent Skills for Claude Code, OpenAI Codex, Cursor, Windsurf, and other AI tools that support `SKILL.md`.

The skills help Czech-speaking non-technical users with repeatable marketing tasks such as copywriting, SEO audits, landing page optimization, e-mail sequences, customer research, social media content, and content strategy.

### Skills included

- `vf-marketingovy-kontext` - shared business and marketing context.
- `vf-copywriting` - Czech marketing copy for websites, landing pages and offers.
- `vf-konverzni-strategie` - conversion diagnosis for offers, pages, e-mails and campaigns.
- `vf-editace-textu` - editing and polishing Czech text.
- `vf-zakaznicky-vyzkum` - customer research questions and synthesis.
- `vf-obsahova-strategie` - content pillars, topics and publishing plans.
- `vf-socialni-obsah` - social media posts for LinkedIn, Facebook, Instagram and X.
- `vf-emailova-sekvence` - onboarding, sales and nurture e-mail sequences.
- `vf-cold-email` - short B2B outreach e-mails and follow-ups.
- `vf-seo-audit` - SEO review for pages, articles and web content.
- `vf-optimalizace-landing-page` - landing page structure and conversion improvements.

Install all skills:

```bash
npx skills add vlastnifiremniai/skills
```

Install selected skills:

```bash
npx skills add vlastnifiremniai/skills --skill vf-konverzni-strategie vf-copywriting vf-seo-audit
```

Start with `vf-marketingovy-kontext`, which creates `.agents/marketingovy-kontext.md`. Other skills use that file as shared business and marketing context.

## Přispívání

Nápady na nové dovednosti, opravy češtiny a zlepšení existujících postupů jsou vítané. Pravidla jsou v [CONTRIBUTING.md](CONTRIBUTING.md).

## Principy dovedností

- Piš česky, jednoduše a konkrétně.
- Neptej se na informace, které už jsou v `.agents/marketingovy-kontext.md`.
- U každého výstupu vysvětli hlavní rozhodnutí krátce a prakticky.
- Nevymýšlej metriky, reference ani zákaznické citace.
