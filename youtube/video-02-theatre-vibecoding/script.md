# Vidéo 02 — Vibe coding (from zero) : « Au théâtre ce soir à Bruxelles »

## Titre (provisoire)
**Je ne sais pas quoi faire avec l’IA… alors je construis un outil utile (théâtre à Bruxelles)**

## Promesse (1 phrase)
En partant d’un vrai problème, on va voir comment l’IA peut aider à **clarifier**, **structurer**, et **construire** une première version d’un outil — même si on n’est pas développeur.

## Intro (texte exact — 30–45s)
Salut, moi c’est Thom.

J’ai 40+, je vis à Bruxelles, et j’ai longtemps eu ce sentiment : “OK l’IA, c’est impressionnant… mais je ne sais pas quoi en faire.”

Donc on va prendre un vrai problème, un truc bête mais réel.
Moi, quand j’ai une soirée libre, je ne sais pas quoi aller voir au théâtre.
Il faut aller sur le site de chaque salle, chercher les dates, comparer… et au final, je renonce.

Aujourd’hui on va voir si on peut construire un mini outil : **"Au théâtre ce soir à Bruxelles"**.
Pas parfait. Juste une première version qui marche.

## Plan (bullets — vibe coding, mais pédagogique)

### 1) Le problème (et pourquoi il est pénible)
- Trop de sites.
- Pas de vue “par date”.
- Pas de filtre simple.
- Les programmations bougent peu → donc scrapable/agrégeable.

### 2) On démarre par la discussion (ChatGPT)
- Décrire le problème en 5 lignes.
- Lister ce qu’on veut voir apparaître : date, théâtre, pièce, heure, lien.
- Clarifier ce qu’on ne fait pas (MVP) : pas de recommandation, pas de comptes, pas de paiement.

### 3) On formalise un PRD (Claude Code)
- User stories simples.
- Scope MVP.
- Sources de données (10 théâtres “scrappables”).
- Contraintes : fiable, pas besoin d’énormes mises à jour.

### 4) On demande une architecture technique (Claude)
- Une base (Supabase) + une table `shows`.
- Un job de collecte (cron/GitHub Actions) qui scrappe et upsert.
- Un front (page web) qui affiche “ce soir / demain / cette semaine”.

### 5) Nouveau repo GitHub
- Structure simple.
- Commits clairs (build in public).

### 6) Première version live
- Une page “Aujourd’hui / date choisie” + liste.
- Un filtre minimal.

### 7) Itération
- On corrige la donnée.
- On améliore l’UI.

## Outro (texte exact — 20–30s)
Si tu as déjà eu ce moment “je ne sais pas quoi faire avec l’IA”, bienvenue.

Si tu es à Bruxelles : dis-moi ton théâtre préféré (ou une salle que tu veux voir dans l’outil).
Et je te montre comment on l’ajoute.
