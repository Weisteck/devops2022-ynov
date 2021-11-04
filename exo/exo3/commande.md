Lancement de la commande docker pour monter un volume :
```bash
docker run -v "$(pwd)/data:/opt" base
```

Pour lancer cette commande il faut avant creer le fichier new-message.txt dans data
