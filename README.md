# Vue3 GitHub Pages

Deploy Vue3 App to GitHub pages.

## Issues and ToDos
- [ ] npm checkout "uses:" stuff doesN#t work with "working dir". mabe set package-lock.json path by hand
- [ ] Want Vue Project in different folder (dev/)
- [ ] Automatic releases
- [X] Use GitHub Actions Secrets
  - [X] Docs how to set it up

## Setup GitHub Action for Deployment to GitHub Pages
#### Step 1: Activate GitHub Pages
- Navigate to GitHub Repository Settings:
- Click on the Settings Tab
- Click Pages
- Select Source: GitHub Actions

#### Step 2: Set Branches to publish from
- In Settings:
- Click Environments
- Click "github-pages"
- Below the list in "Deployment branches and tags" "Add deployment branch or tag rule"
- Type "<YOUR_BRANCH_NAME>"
- Click add rule

#### Step 3: Set Environment Variables / Secrets for GitHub Actions
- In Settings:
- Click "Secrets and variables" > Actions
- Click "New repository secret"
- Add ONE variable & paste the content in the larger text field below
- Click "Add secret"
- Repeat for all your variables

> Ensure these names match those used in your .github/workflows/deploy_to_gh_pages.yaml file.

#### Step 4: Verify Workflow and Deployment
- Ensure `.github/workflows/deploy_to_gh_pages.yaml` is present.
