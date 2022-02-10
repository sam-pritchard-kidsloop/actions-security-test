# actions-security-test

A test project to spike the use of GitHub Actions for CodeQL code scanning, container scans, dependabot, etc. The actions made so far can be seen in the [Actions tab](https://github.com/sam-pritchard-kidsloop/actions-security-test/actions), with the [workflow yaml files in the standard location also](https://github.com/sam-pritchard-kidsloop/actions-security-test/tree/main/.github/workflows).

## CodeQL
A [deliberately vulnerable Go project](https://github.com/0c34/govwa) has been committed to the repository so we can test dependabot and CodeQL scanning. JavaScript has also been added as an option on the scan.

## Dependabot
Dependabot was turned on manually within the [security tab](https://github.com/sam-pritchard-kidsloop/actions-security-test/security).

## TODO

- [x] CodeQL GitHub Actions for GoLang and JavaScript
- [x] Dependabot
- [x] Container scanning
- [x] OpenSSF (GitHub - ossf/scorecard: Security Scorecards - Security health metrics for Open Source )
- [x] Nuclei scans (might need permission to scan something)
- [x] OWASP Zap scans (might need permission to scan something)
- [ ] Investigate if these can be enforced on a global scale or need to be turned on per-repo - if so, we need to automate it with the API and a lambda or something
- [ ] Investigate how we run for multiple languages and tech - is it one workflow per language/tech? It will fail the build if the language isn’t used and we want people to import our standard templates so they don’t have to do the work.
