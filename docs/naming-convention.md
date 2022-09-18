# Naming Convention

## Overview

Use the following naming convention when creating `Terra4GCP64` modules

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

| Google Resource Name | Component (optional) | Alias |
| -------------------- | -------------------- | ----- |
| Organization         |                      | `org` |
| Folder               |                      | `fld` |
| Project              |                      | `prj` |
| Storage              | Bucket               | `sbk` |
| IAM                  | Service Account      | `isa` |
| KMS                  | Key                  | `kky` |
| KMS                  | Ring                 | `krn` |
| Compute Instance     |                      | `ci`  |
| VPC                  | Network              | `vnw` |
| VPC                  | Subnetwork           | `vsn` |
| VPC                  | Route                | `vrt` |
| VPC                  | Firewall             | `vfw` |
| Datacenter           |                      | `dc`  |
