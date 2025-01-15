## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa en document intelligence resurs
```bash
az cognitiveservices account create \
    --name initialerdocument \
    --resource-group airg \
    --kind FormRecognizer \
    --sku F0 \
    --location eastus2 \
    --yes
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```
