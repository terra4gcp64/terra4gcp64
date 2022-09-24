# Naming Convention

## Overview

Use the following naming convention when creating `Terra4GCP64` modules

### Terraform Resource Labels

Use for resource attributes that are used as id or names.

Attribute value: `g-` + **Alias** + `-` + **ResourceAttribute** [+ `-` + **OptionalID**]

Examples:

- `id = "g-isa-account1"`

### Terraform Variables

Variable Name: `g_` + **Alias** + `_` + **ResourceAttribute** [+ `_` + **OptionalID**]

Examples:

- `variable "g_isa_account1"`

### Terraform Output

Output Name: `g_` + **Alias** + `_` + **ResourceAttribute** [+ `_` + **OptionalID**]

Examples:

- `outputs "g_prj_number"`

### Terraform Locals

Local Name for single variable: `g_` + **Alias** + `_` + **ResourceAttribute** [+ `_` + **OptionalID**]

Local Name for complex values:

```text
g_ + **Alias** = {
  **ResourceAttribute** =
}

g_ + **Alias** = {
  **OptionalID** = {
    **ResourceAttribute** =
  }
}
```

Examples:

- `outputs "g_prj_number"`

## Aliases Catalog

| Google Resource Name | Component (optional) | Alias  |
| -------------------- | -------------------- | ------ |
| Compute Instance     |                      | `ci`   |
| Datacenter           |                      | `dc`   |
| Folder               |                      | `fld`  |
| GKE                  | Cluster              | `gkec` |
| IAM                  | Service Account      | `isa`  |
| KMS                  | Key                  | `kky`  |
| KMS                  | Ring                 | `krn`  |
| Organization         |                      | `org`  |
| Project              |                      | `prj`  |
| Storage              | Bucket               | `sbk`  |
| VPC                  | Firewall             | `vfw`  |
| VPC                  | Network              | `vnw`  |
| VPC                  | Route                | `vrt`  |
| VPC                  | Subnetwork           | `vsn`  |
