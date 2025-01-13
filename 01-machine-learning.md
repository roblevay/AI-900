## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg


## Skapa ett machine-learning kommando:

workspace_name="amlws-$RANDOM"
az ml workspace create \
 --name $workspace_name \
 --resource-group airg \
 --location eastus


## Efter labben, ta bort resursgruppen och allt innehåll i den

az group delete --name airg --yes --no-wait
```
