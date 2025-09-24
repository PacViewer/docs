---
title: Blockchain Information
weight: 5
---

List of endpoints for get current details of Pactus blockchain.

### Get Market Cap
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Returns current market cap.

{{< callout type="info" >}}
MarketCap formula

**MarketCap =** Circulation Supply * Last Price

{{< /callout >}}

```
GET https://api.pacviewer.com/v1/marketcap
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
    "status": 200,
    "message": "OK",
    "data": {
        "value": 629447.2329217776
    }
}
  ```

  With `format=text` query:

  ```
  629447.2329217776
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Circulation Supply
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Returns current circulation supply.

{{< callout type="info" >}}
Circulation Supply formula

**Circulation supply =** Total Supply - Total Staked

{{< /callout >}}

```
GET https://api.pacviewer.com/v1/circulation_supply
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
    "status": 200,
    "message": "OK",
    "data": {
        "value": 222983.605938173
    }
}
  ```

  With `format=text` query:

  ```
  222983.605938173
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Total Value Locked (TVL)
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return Total Value Locked (TVL).

{{< callout type="info" >}}
**Total Value Locked (TVL) =**  Total Staked * Last Price

{{< /callout >}}

```
GET https://api.pacviewer.com/v1/total_value_locked
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "value": 439734.2503423898
  }
}
  ```

  With `format=text` query:

  ```
  439734.2503423898
  ```

  {{< /tab >}}

{{< /tabs >}}


### Get Fully Diluted Valuation (FDV)
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return Fully Diluted Valuation (FDV).

{{< callout type="info" >}}
**Fully Diluted Valuation (FDV) =** Max supply * Last Price

{{< /callout >}}

```
GET https://api.pacviewer.com/v1/fully_diluted_valuation
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "value": 840257.9343933696
  }
}
  ```

  With `format=text` query:

  ```
  840257.9343933696
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Total Supply
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return Total supply.

{{< callout type="info" >}}
**Total supply =** Max Supply - Treasury Balance
{{< /callout >}}

```
GET https://api.pacviewer.com/v1/total_supply
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "value": 217541354.1235
  }
}
  ```

  With `format=text` query:

  ```
  217541354.1235
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Max Supply
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return max supply.

{{< callout type="info" >}}
**Max supply =** 42,000,000 PAC
{{< /callout >}}

```
GET https://api.pacviewer.com/v1/max_supply
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "value": 42000000
  }
}
  ```

  With `format=text` query:

  ```
  42000000
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Total Staked
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return Total staked.

{{< callout type="info" >}}
**Total Staked =** total power
{{< /callout >}}

```
GET https://api.pacviewer.com/v1/total_staked
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|
| format | Return value with specific format (text) | text |


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "value":  700059.365163147
  }
}
  ```

  With `format=text` query:

  ```
  700059.365163147
  ```

  {{< /tab >}}

{{< /tabs >}}

### Get Market
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return market details.

```
GET https://api.pacviewer.com/v1/market
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "circulation_supply": 338640.513039625,
    "total_supply": 21798588,
    "total_staked": 697948.304120365,
    "total_value_locked": 830498.4583490798,
    "fully_diluted_valuation": 49976388,
    "volume": 3075.8677,
    "market_cap": 402953.08743303234,
    "price": 1.189914,
    "change_24h": 0,
    "change_7d": 0
  }
}
  ```
  {{< /tab >}}

{{< /tabs >}}

### Get Fee Meter
{{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Return fee details.

```
GET https://api.pacviewer.com/v1/fee
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|


**Headers**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

**Body**

| Key             | Description                                        | Example |
|-----------------|----------------------------------------------------|---------|

  {{< /tab >}}
  {{< tab >}}

  **Status OK 200**

  ```json
{
  "status": 200,
  "message": "OK",
  "data": {
    "since_height": 360,
    "minFee": 2000000,
    "avgFee": 3500000,
    "maxFee": 5000000
  }
}
  ```
  {{< /tab >}}

{{< /tabs >}}