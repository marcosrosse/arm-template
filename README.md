*A REPOSITORY WITH AZURE ARM TEMPLATES EXAMPLES TO STUDY*

arm-template templateFile="azuredeploy.json" 
today=$(date "+%d-%b-%Y")
deploymentName="adeploymentname-"$today

az deployment group create \
--name $deploymentName \
--template-file $templateFile \
--parameters storageAccountType=Standard_LRS storageName=mystorageaccountname