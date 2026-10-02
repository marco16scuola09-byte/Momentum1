# Momentum Daily OS — Sync Edition

## Cosa cambia
- PC e telefono possono usare lo stesso account Supabase.
- I dati principali dell'app vengono sincronizzati nel cloud.
- Il salvataggio locale resta come fallback.
- Login con email/password.
- Non inserire mai una service_role key nel browser.

## Setup
1. Apri il tuo progetto Supabase.
2. Vai in SQL Editor ed esegui `supabase_sync.sql`.
3. Recupera Project URL e Publishable key (oppure anon key compatibile).
4. Pubblica questa cartella su GitHub Pages/HTTPS.
5. Apri l'app, premi `☁️ Sync`, inserisci URL e key.
6. Crea un account oppure accedi.
7. Ripeti l'accesso sul telefono con lo stesso account.

La libreria Supabase viene caricata via CDN. Il browser client usa una sessione persistente; l'accesso database è protetto da RLS per user_id.
