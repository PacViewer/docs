---
title: Blockchain Information
weight: 5
---

List of endpoints for get current details of Pactus blockchain.

### Get Circulation Supply {{< hextra/hero-badge >}} {{< icon name="code" attributes="height=14" >}} Free, No Auth {{< /hextra/hero-badge >}}

Returns current circulation supply.

{{< callout type="info" >}}
Circulation Supply formula ([Pactus FAQs](https://pactus.org/about/faq/#genesis_allocation)):

**Circulation supply =** (Foundation out + VC Allocation out + Team and Operations out + Community out + Team and Operations (Hot) Wallet out + Community (Hot) Wallet out) + Minted - Staked - (Hot)

{{< /callout >}}

```
https://api.pacviewer.com/v1/circulation_supply
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
        "value": 222983.605938173
    }
}
  ```
  {{< /tab >}}

{{< /tabs >}}