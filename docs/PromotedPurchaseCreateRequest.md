# PromotedPurchaseCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PromotedPurchaseCreateRequestData**](PromotedPurchaseCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.promoted_purchase_create_request import PromotedPurchaseCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseCreateRequest from a JSON string
promoted_purchase_create_request_instance = PromotedPurchaseCreateRequest.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseCreateRequest.to_json())

# convert the object into a dict
promoted_purchase_create_request_dict = promoted_purchase_create_request_instance.to_dict()
# create an instance of PromotedPurchaseCreateRequest from a dict
promoted_purchase_create_request_from_dict = PromotedPurchaseCreateRequest.from_dict(promoted_purchase_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


