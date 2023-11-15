# renovate-demo

This repository demonstrates RenovateBot

## Usage

Follow these steps to use this repository:

1. Fork this repository

    After forking explore the repository to understand which outdated dependencies are present.

    Before Renvoate is able to operate on the repository, enable the GitHub App

1. Enable RenovateBot

    The following commands add a configuration for RenovateBot and complete the onboarding process:

    ```bash
    git checkout Onboarding
    git add .
    git commit -m "Enable RenovateBot"
    git push
    ```

1. Configure automerge

    The following commands add a configuration for automerging some dependencies:

    ```bash
    git checkout Automerge
    git add .
    git commit -m "Enable RenovateBot"
    git push
    ```

## Updates to this repository

### Go to beginning

1. Checkout tag `Start`: `git checkout Start`
1. Set branch main: `git branch main --force`
1. Checkout branch `main`: `git checkout main`

### Update demo

1. Update and commit (optionally rebase)
1. Set tag `Start`: `git tag --annotate --message Start Start --force`

### Go to onboarding

1. Copy from tag `Onboarding`: `git checkout Onboarding -- renovate.json`
1. (Optional) Update and commit (optionally rebase)
1. Commit: `git commit --message Onboarding`
1. Set tag `Onboarding`: `git tag --annotate --message Onboarding Onboarding --force`

### Go to automerge

1. Copy from tag `Automerge`: `git checkout Automerge -- renovate.json`
1. (Optional) Update and commit (optionally rebase)
1. Commit: `git commit --message Automerge`
1. Set tag `Automerge`: `git tag --annotate --message Automerge Automerge --force`

### Prepare for usage

1. Return to beginning of demo: `git checkout Start`
1. Reset branch `main`: `git branch main --force`
1. Checkout branch `main`: `git checkout main`
1. Push: `git push --all --force`
