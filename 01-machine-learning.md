## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa ett machine-learning kommando:

```bash
workspace_name="amlws-$RANDOM"
az ml workspace create \
 --name $workspace_name \
 --resource-group airg \
 --location eastus
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```
## Machine-learning-jobbet

Detta jobb tar ungefär 10-15 minuter

## Deploy av Machine-learning-jobbet

Jag använder den virtuella maskinen Standard_D2as_v4 eftersom det inte fanns tillräcklig quota för Standard_DS3_v2.

Deploy tar ca 10 minuter
