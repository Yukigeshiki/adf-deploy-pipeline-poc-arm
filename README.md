# adf-deploy-pipeline-poc-arm
A deploy pipeline PoC for ADF using ARM files.

### Deploy From Local Env

- cd into pipeline directory
- run the following command

```bash
  az deployment group create -g bicpoc-rg-development --template-file Factory.json --parameters @ParametersDevelopment.json
```

### Branching Structure for GitHub Actions Deploy 

- Feature branch e.g. feature/bicpoc1/some-feature
- Enhancement branch e.g. enhancement/bicpoc1/some-enhancement
- Bugfix branch e.g. bugfix/bicpoc1/some-bugfix
- Release branch single pipeline release e.g. release/bicpoc1/2024.12.1
- Release branch multiple pipelines release e.g. release/bicpoc1,bicpoc2,.../2024.12.1