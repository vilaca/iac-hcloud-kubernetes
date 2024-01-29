# iac-hcloud-kubernetes

Deploy Kubernetes on Hetzner Cloud seamlessly using GitHub Actions and [kube-hetzner/terraform-hcloud-kube-hetzner/](https://github.com/kube-hetzner/terraform-hcloud-kube-hetzner).

## Infrastructure as Code (IaC)

The infrastructure code is encapsulated in the [kube.tf](kube.tf) file.

Upon completion of the installation, the kubeconfig.yaml file will be automatically dispatched to a designated email.

## Required Configuration as Secrets

| Action Secret   | Description |
| --------------- | ----------- |
| `HCLOUD_TOKEN`  | Hetzner Cloud API token. Learn how to create it [here](https://docs.hetzner.com/cloud/api/getting-started/generating-api-token/). |
| `MAIL_USERNAME` | Gmail account username. |
| `MAIL_PASSWORD` | Gmail account key (utilize an API key, check [here](https://github.com/dawidd6/action-send-mail) for instructions). |
| `MAIL_TO`       | Email recipient. |

👉🏻 Note: Explore [Action-send-mail](https://github.com/dawidd6/action-send-mail) for options to use other mail providers instead of Gmail.
