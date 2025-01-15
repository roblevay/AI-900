## Skapa en resurs-grupp

```bash
az group create --location eastus --resource-group airg
```

```bash
az cognitiveservices account create \
    --name initialerspeech \
    --resource-group airg \
    --kind SpeechServices \
    --sku F0 \
    --location eastus \
    --yes
```

## Efter labben, ta bort resursgruppen och allt innehåll i den

```bash
az group delete --name airg --yes --no-wait
```





