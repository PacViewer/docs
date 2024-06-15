---
title: Accounts
weight: 6
---

List of endpoints for get current details of accounts.

### Get Account Balance

Returns current balance account.

```
GET https://api.pacviewer.com/v1/accounts/:address/balance
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key     | Description                       | Example |
|---------|-----------------------------------|---------|
| address | account address started with pc1z | pc1z... |


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
  "status": 0,
  "message": "Ok",
  "data": 170750222281
}
  ```

{{< callout type="info" >}}
Data is satoshi type you can convert it to PAC value.

```none
data / 10^9
```

{{< /callout >}}

  {{< /tab >}}

{{< /tabs >}}

### Get Account Details

Returns current account details.

```
GET https://api.pacviewer.com/v1/accounts/:address
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key     | Description                       | Example |
|---------|-----------------------------------|---------|
| address | account address started with pc1z | pc1z... |


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
  "status": 0,
  "message": "Ok",
  "data": {
    "address": "pc1ztlv4af2yt8h2lm965xku8pjsuagcslcee60k6d",
    "hash": "dfa3afe38c2d97fb9d1f8c696b07c5fb7aa90ae3cf40187321f9982ffcdce94e",
    "number": 1321,
    "balance": 170750222281
  }
}
  ```

{{< callout type="info" >}}
Balance is satoshi type you can convert it to PAC value.

```none
balance / 10^9
```

{{< /callout >}}

  {{< /tab >}}

{{< /tabs >}}

### Get Account Transactions

Returns list transactions account.

```
GET https://api.pacviewer.com/v1/accounts/:address/txs?page_no=1&page_size=10
```

{{< tabs items="Request, Response" >}}
  {{< tab >}}
**Query Params**

| Key       | Description                             | Example |
|-----------|-----------------------------------------|---------|
| address   | account address started with pc1z       | pc1z... |
| page_no   | set page number (default is 1)          | 1       |
| page_size | set page size (optional, default is 10) | 10      |


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
"status": 0,
"message": "Ok",
"data": {
  "page_no": 1,
  "page_size": 10,
  "total_items": 9240,
  "data": [
      {
        "id": "666d2ac2820a482468641c96",
        "hash": "d9f5ead33f20cb93dc6333206b457365942b651510bec06934fb8c9ee79e007c",
        "blockHeight": 1173686,
        "version": 1,
        "type": 1,
        "from": "",
        "to": "pc1ztlv4af2yt8h2lm965xku8pjsuagcslcee60k6d",
        "value": 1000000000,
        "fee": 0,
        "memo": "",
        "signature": "",
        "createdAt": "2024-06-15T05:46:40Z"
      },
      {
        "id": "666d291e820a482468641b28",
        "hash": "24e6b2a169fadefd73517133427bf1f4425dd983747e53fccc4b4a0e0128e9e2",
        "blockHeight": 1173644,
        "version": 1,
        "type": 1,
        "from": "",
        "to": "pc1ztlv4af2yt8h2lm965xku8pjsuagcslcee60k6d",
        "value": 1000000000,
        "fee": 0,
        "memo": "",
        "signature": "",
        "createdAt": "2024-06-15T05:39:40Z"
      }
    ]
  }
}
  ```

{{< callout type="info" >}}
Note: result transactions is Z-A base on created at.
{{< /callout >}}

  {{< /tab >}}

{{< /tabs >}}
