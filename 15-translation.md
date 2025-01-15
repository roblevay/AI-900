## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

## Skapa en translator-resurs

```bash
az cognitiveservices account create \
    --name initialertranslator \
    --resource-group airg \
    --kind Translator \
    --sku S1 \
    --location eastus \
    --yes
```



## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```

