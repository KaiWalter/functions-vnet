# Functions VNET
Simple Functions container to test operations for locked down virtual network scenarios.

## build test container

```
docker build . -t ancientitguy/functions-vnet
```

## run test container

create `dev.env` file in the format
```env
APPINSIGHTS_INSTRUMENTATIONKEY=...app insights key...
STORAGE_ACCOUNT=...storage account url...
```

```
docker run -d -p 5001:5001 --env-file ./dev.env ancientitguy/functions-vnet
```

