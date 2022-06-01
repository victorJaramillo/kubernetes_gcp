# Kubernetes
### Para no tener que usar el comando kubectl, tengo un alias en mi máquina, referenciado como 'k'.
````
alias k='kubectl'
````

## Aplicar pod
```
k apply -f 03-ubuntu-pod.yml
```

# Aplicar deployment
```
k apply -f 04-ubuntu-deployment.yml
```

# Entrar en modo bash al pod
```
k exec --stdin --tty ubuntu -- /bin/bash
k exec --stdin --tty ${POD_ID} -- /bin/bash
```

# Extender replicas(manual)
```
k scale --replicas=3 Deployment/ubuntu
```

<p align="center">Copyright © 2022 vjdev</p>