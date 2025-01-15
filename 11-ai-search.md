




az search service create \
    --name initialersearch \
    --resource-group airg \
    --sku Basic \
    --location eastus


az cognitiveservices account create \
    --name initialerservices \
    --resource-group airg \
    --kind OpenAI \
    --sku S0 \
    --location eastus \
    --yes
