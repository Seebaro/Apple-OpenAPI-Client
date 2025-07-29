# InAppPurchaseV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseV2Attributes**](InAppPurchaseV2Attributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseV2Relationships**](InAppPurchaseV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2 import InAppPurchaseV2

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2 from a JSON string
in_app_purchase_v2_instance = InAppPurchaseV2.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2.to_json())

# convert the object into a dict
in_app_purchase_v2_dict = in_app_purchase_v2_instance.to_dict()
# create an instance of InAppPurchaseV2 from a dict
in_app_purchase_v2_from_dict = InAppPurchaseV2.from_dict(in_app_purchase_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


