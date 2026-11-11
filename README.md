# mathaid-legal

Page publique de politique de confidentialité pour l'app Leo (MathAidApp).

## Étapes pour publier avec GitHub Pages

1. Ouvre `index.html` et remplace les deux `[À COMPLÉTER]` (identité de
   l'éditeur, email de contact), puis supprime le bloc jaune "À compléter".
2. Crée un dépôt GitHub **public** nommé par exemple `mathaid-legal`.
3. Depuis ce dossier :
   ```
   git init
   git add index.html README.md
   git commit -m "Politique de confidentialité"
   git branch -M main
   git remote add origin https://github.com/<ton-pseudo>/mathaid-legal.git
   git push -u origin main
   ```
4. Sur GitHub : Settings → Pages → Source : "Deploy from a branch" →
   Branch : `main` / `/(root)`. Après quelques minutes, la page est
   disponible à `https://<ton-pseudo>.github.io/mathaid-legal/`.
5. Renseigne cette URL :
   - Dans App Store Connect : App Information → Privacy Policy URL, et
     dans la fiche de l'abonnement (Subscriptions) → Privacy Policy URL.
   - Dans l'app (déjà fait par Claude) : `AuthView.swift` et
     `PaywallView.swift`.

## CGU (Conditions Générales d'Utilisation)

Pas besoin d'héberger de CGU personnalisées : l'app utilise l'EULA
standard fournie gratuitement par Apple, qui couvre les exigences
d'App Store Connect (règle 3.1.2) :

https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

Cette URL est déjà celle utilisée par défaut par Apple si aucune EULA
personnalisée n'est renseignée dans App Store Connect — il n'y a donc
rien à configurer côté App Store Connect pour ça. Le lien a simplement
été ajouté dans l'app (AuthView, PaywallView) pour que l'utilisateur
puisse le consulter avant de créer un compte ou de s'abonner.
