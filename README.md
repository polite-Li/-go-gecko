
[Refer to CoinGecko official API](https://www.coingecko.com/api)


## Usage

Installation with go get.

```
go get -u github.com/polite-Li/go-gecko
```

For usage, checkout [Example folder for v3](/_example/v3)

For production, you might need to set time out for httpClient, here's a sample code:

```go
package main

import (
	"net/http"
	"time"

	coingecko "github.com/polite-Li/go-gecko/v3"
)

func main() {
	httpClient := &http.Client{
		Timeout: time.Second * 10,
	}
	CG := coingecko.NewClient(httpClient)
}
```

## Convention

refer to https://medium.com/@marcus.olsson/writing-a-go-client-for-your-restful-api-c193a2f4998c

## License

MIT
