
## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa ett machine-learning kommando:

```bash
az cognitiveservices account create \
  --name initialermymultiaccount \
  --resource-group airg \
  --kind CognitiveServices \
  --sku S0 \
  --location eastus \
  --yes
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```
