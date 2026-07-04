# Návod – správa galerie bez zásahu do kódu

## 1) Nahrání na GitHub
1. Na GitHubu jsi vytvořil repozitář (např. `kompleto-web`).
2. Na stránce repa klikni na **"uploading an existing file"** (nebo Add file → Upload files).
3. Přetáhni tam VŠECHNY soubory a složky z tohoto balíčku (zachovej strukturu složek: `admin/`, `data/`, `images/`, `index.html`).
4. Dole napiš commit zprávu (např. "první nahrání") a klikni **Commit changes**.

## 2) Propojení GitHubu s Netlify
1. Jdi na svůj Netlify projekt → **Site configuration** (nebo Project configuration).
2. Najdi **Build & deploy** → **Link repository** / **Link site to Git**.
3. Vyber GitHub, přihlas se, vyber repozitář `kompleto-web`.
4. Build command nech prázdný, Publish directory nastav na `/` (kořen). Ulož.
5. Netlify od teď bude nasazovat web automaticky při každé změně v repu.

## 3) Zapnutí přihlašování (Netlify Identity)
1. V Netlify jdi do svého projektu → **Identity** (pokud tam záložka není, najdeš ji přes horní menu nebo Site configuration → Identity).
2. Klikni **Enable Identity**.
3. Dole v sekci **Registration** nastav na **Invite only** (ať se nemůže zaregistrovat kdokoliv z internetu).
4. Najdi sekci **Services → Git Gateway** a klikni **Enable Git Gateway**.
5. V záložce Identity klikni **Invite users** a pozvi svůj vlastní e-mail. Přijde ti pozvánka, přes kterou si nastavíš heslo.

## 4) Použití
1. Jdi na `https://tvuj-web.netlify.app/admin/`
2. Přihlas se e-mailem a heslem, které sis nastavil.
3. V sekci **Galerie prací** můžeš přidávat, mazat a upravovat fotky — nahraješ obrázek, napíšeš popisek, vybereš kategorii.
4. Po uložení Netlify samo nasadí novou verzi webu (chvíli to trvá, cca 1 minutu).

## Poznámka
Pár fotek (placeholder z picsum.photos) tam je jen jako ukázka — v adminu je klidně smaž a nahraď svými skutečnými fotkami zakázek.
