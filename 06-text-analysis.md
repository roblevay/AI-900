## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa language-resurs

```bash
az cognitiveservices account create \
  --name <ditt-unika-namn> \
  --resource-group airg \
  --kind Language \
  --sku F0 \
  --location eastus \
  --yes \
  --api-properties "[]" \
  --tags Purpose=LanguageService
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
