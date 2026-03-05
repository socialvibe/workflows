# Workflows

Repository to host shared company workflows, GitHub Actions, and PR templates for Infillion repositories.

## Contents

### GitHub Actions Workflows

Located in `.github/workflows/`:

* **`pr_jira_ticket.yml`**: A GitHub Action workflow that enforces Pull Request titles to begin with a valid Jira project ticket ID (e.g., `DSOS-1234: <description>`). It ensures the title is prefixed correctly.
* **`pr_jira_ticket_mm.yml`**: A more permissive version of the PR title check that allows the Jira ticket ID to be placed anywhere in the PR title, such as `fix(PROJECT-123): <description>`. It also automatically skips the check on push events.

### Templates

Located in `.github/`:

* **`pull_request_template.md`**: A standardized Pull Request template to ensure consistent documentation across PRs. It includes required sections for:
  * **What Will Change**
  * **Why It Will Change**
  * **Affected Systems**
  * **Rollback Process**
  * **Related Links** (Jira)
