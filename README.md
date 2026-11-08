# iAvirix: aggiornamenti

Questo repository serve il sito statico `https://updates.iavirix.com` tramite GitHub Pages.
Contiene solo materiale pubblico per natura:

- `appcast.xml`: feed Sparkle firmato EdDSA (la chiave pubblica è compilata nell'app).
- `releases/`: i DMG firmati Developer ID e notarizzati, con gli hash SHA-256 di ogni versione.

Nessun file viene scritto a mano: li pubblica il workflow "Pubblica feed" del repository privato
`tonyxus/iAvirix` quando una GitHub Release passa da bozza a pubblicata. Modifiche manuali a questo
repository vengono sovrascritte alla pubblicazione successiva.

Il feed non è un canale di fiducia: Sparkle accetta un aggiornamento solo se la firma EdDSA
dell'appcast corrisponde alla chiave pubblica compilata nell'app e se il DMG è firmato e notarizzato.
