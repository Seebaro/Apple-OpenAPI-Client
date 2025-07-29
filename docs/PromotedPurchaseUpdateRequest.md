# PromotedPurchaseUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PromotedPurchaseUpdateRequestData**](PromotedPurchaseUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.promoted_purchase_update_request import PromotedPurchaseUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseUpdateRequest from a JSON string
promoted_purchase_update_request_instance = PromotedPurchaseUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseUpdateRequest.to_json())

# convert the object into a dict
promoted_purchase_update_request_dict = promoted_purchase_update_request_instance.to_dict()
# create an instance of PromotedPurchaseUpdateRequest from a dict
promoted_purchase_update_request_from_dict = PromotedPurchaseUpdateRequest.from_dict(promoted_purchase_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


