# Google Cloud Terraform Initial Setup

## Requirements
- Project Admin on a Google Cloud project
- `gcloud` cli installed (for troubleshooting)
- `terraform` >= 0.13.2

## Scope
This tutorial will prepare us for provisioning resources using Google Compute Cloud (GCP) Compute Engine. As such, we will be granting permissions to a service account to work with these resources.

## Preparing Environment
In order to be able to interact with our GCP project using `terraform`, we will need a service account.

For the purpose of this tutorial, we will create a service account with a lot of permissions to make getting started easy.

In a production environment, however, we will want to make sure we make very specific service account roles based upon which resources they will be editing.

### Roles
- Compute Admin
  - Allows access to `compute.*`, which includes all compute engine resources such as storage, zones, instances, networking, etc.



