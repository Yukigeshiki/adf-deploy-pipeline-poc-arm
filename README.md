# adf-deploy-pipeline-poc-arm
A deploy pipeline PoC for ADF using ARM files.

### Deploy From Local Env

az deployment group create -g bicpoc-rg-development --template-file Factory.json --parameters @ParametersDevelopment.json
