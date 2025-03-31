# practicaKube

- Añadidos archivos de creaciòn de pods usando
    - ReplicaContainer
    - ReplicaSet
    - Deployment

- Comandos importantes de kubernetes
    - Aplicar un archivo yaml: kubectl apply -f dptest.yaml
    - Borrar un deployment: kubectl delete deployment app1-dp
    - Obtener el listado de pods: kubectl get pods 
    - Obtener todos los pods: kubectl get all
    - Describir pods: kubectl describe <nombre del pod>
    - Borrar pod: kubectl delete pod <nombre del pod>
    - Bajar o subir el número de réplicas de pod: kubectl scale deploy/app1 --replicas 5
    - Ver el estado de un rollout de deployment: kubectl rollout status deploy/app1
    - Rollback a una versión anterior de deploy: kubectl rollout undo deployment/aplicacion
    - Exponer servicios para que los ocupen otras aplicaciones: kubectl expose
    - Ver los namespaces: kubectl get namespaces
    - Crear configmap desde archivo: kubectl create configmap --from-file=<nombre de archivo>
    - Crear secret por archivo: kubectl create secret generic db-user-pass --from-file=./username.txt --from-file=.password.txt 
    - Crear secret por linea de comando: kubectl create secret generic db-user-pass --from-literal=username=admin --from-literal=password='password'
    - Borrar secreto: kubectl delete secret db-user-pass
    
