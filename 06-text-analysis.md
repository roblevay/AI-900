

az cognitiveservices account create \
  --name <ditt-unika-namn> \
  --resource-group airg \
  --kind Language \
  --sku F0 \
  --location eastus \
  --yes \
  --api-properties "[]" \
  --tags Purpose=LanguageService
