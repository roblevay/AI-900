## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa content safety resurs

```bash
az cognitiveservices account create \
    --name $(openssl rand -hex 8) \
    --resource-group airg \
    --location eastus \
    --kind ContentSafety \
    --sku S0 \
    --yes
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```
