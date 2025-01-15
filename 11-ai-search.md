## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa en search resurs
```bash
az search service create \
    --name initialersearch \
    --resource-group airg \
    --sku Basic \
    --location eastus
```

## Skapa en services resurs
```bash
az cognitiveservices account create \
    --name initialerservices \
    --resource-group airg \
    --kind OpenAI \
    --sku S0 \
    --location eastus \
    --yes
```

## Skapa storage konto
```bash
az storage account create \
    --name initialerstorage \
    --resource-group airg \
    --location eastus2 \
    --sku Standard_LRS \
    --kind StorageV2
```

## Tillåt anonym åtkomst
```bash
az storage account update \
    --name initialerstorage \
    --resource-group airg \
    --set allowBlobPublicAccess=true
```


## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```








