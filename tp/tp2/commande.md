Pour tester le loadbalancer en mettant des fichier index html :
```
kubectl create cm index1 --from-file=index.html=index1.html
```

Astuce du petit Kevin : `Ctrl+Shift+r` -> vider le cache et refresh
