# InAppPurchaseAvailabilityCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseAvailabilityCreateRequestData**](InAppPurchaseAvailabilityCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_availability_create_request import InAppPurchaseAvailabilityCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAvailabilityCreateRequest from a JSON string
in_app_purchase_availability_create_request_instance = InAppPurchaseAvailabilityCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAvailabilityCreateRequest.to_json())

# convert the object into a dict
in_app_purchase_availability_create_request_dict = in_app_purchase_availability_create_request_instance.to_dict()
# create an instance of InAppPurchaseAvailabilityCreateRequest from a dict
in_app_purchase_availability_create_request_from_dict = InAppPurchaseAvailabilityCreateRequest.from_dict(in_app_purchase_availability_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


