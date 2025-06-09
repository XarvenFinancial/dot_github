# .github Repository

Supports various integrations for templating source control resources.

- **Default community health files**  
  By creating a public `.github` repo, you can supply organization-wide defaults for community-health documents:  
  - `CODE_OF_CONDUCT.md`  
  - `CONTRIBUTING.md`  
  - `SECURITY.md`  
  - `SUPPORT.md`  
  - `FUNDING.yml`  
  - `GOVERNANCE.md`  
  - Default issue & pull-request templates (see below)  
  

- **Issue & Pull Request templates + chooser config**  
  Store templates in these hidden folders on your default branch to standardize new-issue and new-PR forms across every repo:  
  - `.github/ISSUE_TEMPLATE/` (multiple `.md` or form-schema `.yml` files)  
  - `.github/PULL_REQUEST_TEMPLATE/` (multiple templates via subdirectory)  
  - `.github/ISSUE_TEMPLATE/config.yml` to control the issue-template chooser UI  
  

- **Discussion category forms**  
  Define custom discussion templates (with GitHub’s form schema) by adding YAML files to  
  `.github/DISCUSSION_TEMPLATE/`, so organization-level Discussions use structured forms.  
  

- **Organization profile README**  
  Customize your org’s public profile page by committing a `profile/README.md` inside `.github`.  
  

- **Workflow templates**  
  In `.github/workflow-templates/`, you can publish starter GitHub Actions workflows for your team. Each template gets a companion `.properties.json` for name, description, icon, categories, and file-pattern matching:  
  ```text
  .github/
    └─ workflow-templates/
         ├─ my-ci.yml
         └─ my-ci.properties.json
  ```  
  

- **Reusable workflows**  
  Place reusable workflow files under `.github/workflows/` in your org repo, then call them from any repo in your organization to enforce consistent automation.  
  

- **Dependabot configuration**  
  Add a single `dependabot.yml` at the root of `.github/` to enable and configure Dependabot version-update PRs across all your org’s repositories.  
  

- **CODEOWNERS**  
  Define a central `.github/CODEOWNERS` file to automatically request reviews from specified users or teams whenever certain paths change, organization-wide.  
  
