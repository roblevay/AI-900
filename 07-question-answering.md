## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa language-resurs

```bash
az cognitiveservices account create \
  --name initialermylanguage \
  --resource-group airg \
  --kind TextAnalytics \
  --sku S \
  --location eastus \
  --yes

```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```

