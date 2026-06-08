# wordpress-gitops-kind

Manifests Kubernetes (WordPress + MySQL, images officielles) déployés en GitOps
par ArgoCD sur des clusters kind locaux.

- `manifests/mysql.yaml` — MySQL 8.0 (Secret, Deployment headless, Service)
- `manifests/wordpress.yaml` — WordPress 6.5 (Deployment + Service ClusterIP)

Chaque cluster kind possède son ArgoCD qui synchronise ce dépôt vers le
namespace `wordpress`.
