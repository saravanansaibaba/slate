---
title: Card Data API v1

search: true
---

# Card Data API v1
> ### Produces


## 

```http
GET //api/CardData HTTP/1.1
Content-Type: application/json

{
    "cardDataRequest": {
        "fiid": "string",
        "bin": "string",
        "cardNumber": "string"
    }
}
```
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "fiid": "string",
    "bin": "string",
    "cardNumber": "string",
    "accountOpenedDate": "string",
    "branchId": "string",
    "cardHolder": {
        "firstName": "string",
        "lastName": "string",
        "email": "string",
        "addressVerificationZip": "string",
        "primaryPhone": "string"
    }
}
```

### Parameters
Name | In | Type | Description
--- | --- | --- | ---
cardDataRequest | body | [CardDataRequest](#carddatarequest) | 
//todo: migrate to html tables. after cool looking nested table
### Responses
<span comment="workaround for markdown processing in table"></span>
<table>
<tr><th>Http code</th><th>Type</th><th>Description</th></tr>
<tr><td>200</td><td>[CardData](#carddata)</td><td>OK</td></tr> 
</table>
## 

```http
PUT //api/CardData HTTP/1.1
Content-Type: application/json

{
    "cardDataRequest": {
        "fiid": "string",
        "bin": "string",
        "cardNumber": "string"
    }
}
```
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "fiid": "string",
    "bin": "string",
    "cardNumber": "string",
    "accountOpenedDate": "string",
    "branchId": "string",
    "cardHolder": {
        "firstName": "string",
        "lastName": "string",
        "email": "string",
        "addressVerificationZip": "string",
        "primaryPhone": "string"
    }
}
```

### Parameters
Name | In | Type | Description
--- | --- | --- | ---
cardDataRequest | body | [CardDataRequest](#carddatarequest) | 
//todo: migrate to html tables. after cool looking nested table
### Responses
<span comment="workaround for markdown processing in table"></span>
<table>
<tr><th>Http code</th><th>Type</th><th>Description</th></tr>
<tr><td>200</td><td>[CardData](#carddata)</td><td>OK</td></tr> 
</table>
## 

```http
POST //api/CardData HTTP/1.1
Content-Type: application/json

{
    "createCardRequest": {
        "fiid": "string",
        "bin": "string",
        "branchId": "string",
        "cardHolder": {
            "firstName": "string",
            "lastName": "string",
            "email": "string",
            "addressVerificationZip": "string",
            "primaryPhone": "string"
        }
    }
}
```
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "fiid": "string",
    "bin": "string",
    "cardNumber": "string",
    "accountOpenedDate": "string",
    "branchId": "string",
    "cardHolder": {
        "firstName": "string",
        "lastName": "string",
        "email": "string",
        "addressVerificationZip": "string",
        "primaryPhone": "string"
    }
}
```

### Parameters
Name | In | Type | Description
--- | --- | --- | ---
createCardRequest | body | [CreateCardRequest](#createcardrequest) | 
//todo: migrate to html tables. after cool looking nested table
### Responses
<span comment="workaround for markdown processing in table"></span>
<table>
<tr><th>Http code</th><th>Type</th><th>Description</th></tr>
<tr><td>200</td><td>[CardData](#carddata)</td><td>OK</td></tr> 
</table>
## 

```http
DELETE //api/CardData HTTP/1.1
Content-Type: application/json

{
    "cardDataRequest": {
        "fiid": "string",
        "bin": "string",
        "cardNumber": "string"
    }
}
```
```http
HTTP/1.1 204 No Content
```

### Parameters
Name | In | Type | Description
--- | --- | --- | ---
cardDataRequest | body | [CardDataRequest](#carddatarequest) | 
//todo: migrate to html tables. after cool looking nested table
### Responses
<span comment="workaround for markdown processing in table"></span>
<table>
<tr><th>Http code</th><th>Type</th><th>Description</th></tr>
<tr><td>204</td><td>no content</td><td>No Content</td></tr> 
</table>


# Models
## CardDataRequest
```json
{
    "fiid": "string",
    "bin": "string",
    "cardNumber": "string"
}
```
	
### Fields
Name | Type | Description
--- | --- | ---
fiid<b title="required">&nbsp;*&nbsp;</b> | string | 
bin<b title="required">&nbsp;*&nbsp;</b> | string | 
cardNumber<b title="required">&nbsp;*&nbsp;</b> | string | 

	
## CardData
```json
{
    "fiid": "string",
    "bin": "string",
    "cardNumber": "string",
    "accountOpenedDate": "string",
    "branchId": "string",
    "cardHolder": {
        "firstName": "string",
        "lastName": "string",
        "email": "string",
        "addressVerificationZip": "string",
        "primaryPhone": "string"
    }
}
```
	
### Fields
Name | Type | Description
--- | --- | ---
fiid<b title="required">&nbsp;*&nbsp;</b> | string | 
bin<b title="required">&nbsp;*&nbsp;</b> | string | 
cardNumber<b title="required">&nbsp;*&nbsp;</b> | string | 
accountOpenedDate | string | 
branchId | string | 
cardHolder | [CardHolder](#cardholder) | 

	
## CardHolder
```json
{
    "firstName": "string",
    "lastName": "string",
    "email": "string",
    "addressVerificationZip": "string",
    "primaryPhone": "string"
}
```
	
### Fields
Name | Type | Description
--- | --- | ---
firstName<b title="required">&nbsp;*&nbsp;</b> | string | 
lastName<b title="required">&nbsp;*&nbsp;</b> | string | 
email<b title="required">&nbsp;*&nbsp;</b> | string | 
addressVerificationZip | string | 
primaryPhone | string | 

	
## CreateCardRequest
```json
{
    "fiid": "string",
    "bin": "string",
    "branchId": "string",
    "cardHolder": {
        "firstName": "string",
        "lastName": "string",
        "email": "string",
        "addressVerificationZip": "string",
        "primaryPhone": "string"
    }
}
```
	
### Fields
Name | Type | Description
--- | --- | ---
fiid<b title="required">&nbsp;*&nbsp;</b> | string | 
bin<b title="required">&nbsp;*&nbsp;</b> | string | 
branchId<b title="required">&nbsp;*&nbsp;</b> | string | 
cardHolder | [CardHolder](#cardholder) | 

	
