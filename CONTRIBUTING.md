# Contributing

## Development

### Environment

- Prepare dev tools:
  - Install the latest version of the [Terraform CLI](https://www.terraform.io/downloads)
  - Install GIT
  - (Optional) Install Git Flow
- Clone GIT repositories

  ```shell
  # Create the main repository
  cd <YOUR_PROJECTS_PATH>
  git clone https://github.com/serdigital64/terra4gcp64.git
  cd terra4gcp64
  # Create module repositories as git submodules
  git submodule init
  # Update modules
  git submodule update
  # Enable main branch on submodules
  git submodule foreach "git checkout main"; git submodule foreach "git checkout develop"
  # (Optional) Initialize git flow. Production branch:main, use defaults for the remaining branches
  git submodule foreach "git flow init"
  ```

- Adjust environment variables to reflect your configuration:

  ```shell
  # Copy environment definition files from templates:
  cp dot.local .local
  cp dot.secrets .secrets
  # Review and update content for both files
  ```

- Initialize dev environment variables

  ```shell
  source bin/devta-set
  ```

## Repositories

- Project GIT repository: [https://github.com/serdigital64/terra4gcp64](https://github.com/serdigital64/terra4gcp64)
- Project Documentation: [https://github.com/serdigital64/terra4gcp64](https://github.com/serdigital64/terra4gcp64)
- Terraform Namespace: [https://registry.terraform.io/namespaces/terra4gcp64](https://registry.terraform.io/namespaces/terra4gcp64)
