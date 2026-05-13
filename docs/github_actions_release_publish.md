# GitHub Actions Release Publish

## Goal

Define the GitHub Actions workflow that updates this catalog from private plugin or theme source repositories.

## Required Behavior

- workflow runs from the private source repo
- workflow builds artifacts
- workflow checks out this public catalog repo with write access
- workflow copies artifacts and metadata into the right version directory
- workflow runs catalog validation
- workflow commits and pushes the catalog update

## Security Notes

- use a scoped token or deploy key with write access only to this catalog repo
- do not expose private source code in artifacts
- avoid writing secrets into logs

## Done When

- release publication from private repos into this public catalog is automated and repeatable
