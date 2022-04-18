# kubernetes-postgresql
Kubernetes PostgreSQL Deployment

## Namespace for test and prod environments
test/database-test-namespace.yaml
prod/database-prod-namespace.yaml

## PersistentVolume using NFS storage 
Change NFS server IP and path
test/postgresql-test-pv.yaml
prod/postgresql-prod-pv.yaml

## PersistentVolumeClaim
test/postgresql-test-pvc.yaml
prod/postgresql-prod-pvc.yaml

## ConfigMap for credentials 
Very \!/ not secure but you can change the password on first connection
test/postgresql-test-configmap.yaml
prod/postgresql-prod-configmap.yaml

## Deployment of pgAdmin
test/postgresql-test-deployment.yaml
prod/postgresql-prod-deployment.yaml

## Services
test/postgresql-test-clusterip-service.yaml
prod/postgresql-prod-clusterip-service.yaml


## Alls files in one
test/postgresql-test.yaml
prod/postgresql-prod.yaml
