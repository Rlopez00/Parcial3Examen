# Proyecto: WordPress en Amazon EKS con almacenamiento persistente (EBS + EFS)

Este proyecto despliega un sitio WordPress usando Amazon Elastic Kubernetes Service (EKS).
Incluye almacenamiento persistente:
- MySQL sobre Amazon EBS
- WordPress sobre Amazon EFS

## 🚀 Instrucciones de despliegue

### Prerequisitos:
- AWS CLI configurado
- kubectl instalado
- helm instalado
- Un clúster Amazon EKS activo

### Pasos:

1. Crear el Secret para la contraseña de MySQL:
   ```bash
   kubectl create secret generic mysql-pass --from-literal=password=TuPasswordSegura
