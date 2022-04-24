# kubernetes-APP
Kubernetes objects for APP deployment

# kubernetes-postgresql
Kubernetes object for PostgreSQL deployment


# Namespaces
## database test Namespace
test/database-test-Namespace.yaml
## database prod Namespace
prod/database-prod-Namespace.yaml


# ConfigMaps
Very \!/ not secure but you can change the password on first connection
## PostgreSQL test ConfigMap
test/postgresql-test-ConfigMap.yaml
## PostgreSQL prod ConfigMap
prod/postgresql-prod-ConfigMap.yaml


# RBAC
## APP ClusterRole
APP-ClusterRole.yaml

## APP ClusterRoleBinding
APP-ClusterRoleBinding.yaml

## APP Role
APP-Role.yaml

## APP RoleBinding
APP-RoleBinding.yaml


# Storages
## PostgreSQL test PersistentVolume using NFS storage 
Change NFS server IP and path
test/postgresql-test-PersistentVolume-nfs.yaml
## PostgreSQL prod PersistentVolume using NFS storage 
prod/postgresql-prod-PersistentVolume-nfs.yaml

## PersistentVolumeClaim
## PostgreSQL test PersistentVolumeClaim using NFS PersistentVolume
test/postgresql-test-PersistentVolumeClaim-nfs.yaml
## PostgreSQL prod PersistentVolumeClaim using NFS PersistentVolume
prod/postgresql-prod-PersistentVolumeClaim-nfs.yaml


# Deployments
## PostgreSQL test Deployment using NFS storage
test/postgresql-test-deployment-nfs.yaml
## PostgreSQL prod Deployment using NFS storage
prod/postgresql-prod-deployment-nfs.yaml


# Services
Use one of them (I use LoadBalancer with MetalLB on my private cluster)
## PostgreSQL test LoadBalancer Service
test/postgresql-test-Service-LoadBalancer-service.yaml
## PostgreSQL prod LoadBalancer Service
prod/postgresql-prod-Service-LoadBalancer-service.yaml

## PostgreSQL test ClusterIP Service
test/postgresql-test-Service-ClusterIP-service.yaml
## PostgreSQL prod ClusterIP Service
prod/postgresql-prod-Service-ClusterIP-service.yaml