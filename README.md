# Libro Informatica SIA — repository sorgente

Il libro è scritto in Markdown (cartella `docs/`, un file per capitolo).
A ogni push su `main`, GitHub costruisce e pubblica automaticamente il sito.

## Messa online (una volta sola, ~10 minuti)

1. Crea un repository su GitHub (es. `libro-sia`), anche privato: il sito può comunque essere pubblico.
2. Carica il contenuto di questa cartella nel repository (da browser: "uploading an existing file", trascina tutto; oppure con git da terminale).
3. Al primo push l'Action "Pubblica il sito" parte da sola (scheda **Actions**).
4. Quando finisce: **Settings → Pages → Branch: `gh-pages`** → Save.
5. Il sito è su `https://TUOUTENTE.github.io/libro-sia/` — questo è il link da dare agli studenti.

## Anteprima locale (facoltativa)

    pip install mkdocs-material
    mkdocs serve        # sito di anteprima su http://127.0.0.1:8000

## Aggiungere un capitolo

1. Nuovo file `docs/capitolo-N.md`
2. Una riga nella sezione `nav:` di `mkdocs.yml`
3. Push → il sito si aggiorna da solo.

## Box del libro

I box colorati sono "admonition": `!!! example "Esempio 1"` con il contenuto
indentato di 4 spazi. Tipi usati: `abstract` (definizione), `info` (sintassi),
`example`, `note`, `tip` (curiosità), `warning` (attenzione), `question` (esercizi).
Le risposte nascoste usano `??? question "Risposte corrette"` (collassabile).
