# actions-security-test

A test project to spike the use of GitHub Actions for CodeQL code scanning, container scans, dependabot, etc. The actions made so far can be seen in the [Actions tab](https://github.com/sam-pritchard-kidsloop/actions-security-test/actions), with the [workflow yaml files in the standard location also](https://github.com/sam-pritchard-kidsloop/actions-security-test/tree/main/.github/workflows).

## CodeQL
A [deliberately vulnerable Go project](https://github.com/0c34/govwa) has been committed to the repository so we can test dependabot and CodeQL scanning. JavaScript has also been added as an option on the scan.

## Dependabot
Dependabot was turned on manually within the [security tab](https://github.com/sam-pritchard-kidsloop/actions-security-test/security).
