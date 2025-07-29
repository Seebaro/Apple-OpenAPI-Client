# InAppPurchaseAvailabilityCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppAvailabilityV2CreateRequestDataAttributes**](AppAvailabilityV2CreateRequestDataAttributes.md) |  | 
**relationships** | [**InAppPurchaseAvailabilityCreateRequestDataRelationships**](InAppPurchaseAvailabilityCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_availability_create_request_data import InAppPurchaseAvailabilityCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAvailabilityCreateRequestData from a JSON string
in_app_purchase_availability_create_request_data_instance = InAppPurchaseAvailabilityCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAvailabilityCreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_availability_create_request_data_dict = in_app_purchase_availability_create_request_data_instance.to_dict()
# create an instance of InAppPurchaseAvailabilityCreateRequestData from a dict
in_app_purchase_availability_create_request_data_from_dict = InAppPurchaseAvailabilityCreateRequestData.from_dict(in_app_purchase_availability_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


