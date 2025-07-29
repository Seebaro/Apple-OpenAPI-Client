# InAppPurchaseAvailability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppAvailabilityV2Attributes**](AppAvailabilityV2Attributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseAvailabilityRelationships**](InAppPurchaseAvailabilityRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_availability import InAppPurchaseAvailability

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAvailability from a JSON string
in_app_purchase_availability_instance = InAppPurchaseAvailability.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAvailability.to_json())

# convert the object into a dict
in_app_purchase_availability_dict = in_app_purchase_availability_instance.to_dict()
# create an instance of InAppPurchaseAvailability from a dict
in_app_purchase_availability_from_dict = InAppPurchaseAvailability.from_dict(in_app_purchase_availability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


