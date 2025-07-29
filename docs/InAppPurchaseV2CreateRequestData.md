# InAppPurchaseV2CreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**InAppPurchaseV2CreateRequestDataAttributes**](InAppPurchaseV2CreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_v2_create_request_data import InAppPurchaseV2CreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2CreateRequestData from a JSON string
in_app_purchase_v2_create_request_data_instance = InAppPurchaseV2CreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2CreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_v2_create_request_data_dict = in_app_purchase_v2_create_request_data_instance.to_dict()
# create an instance of InAppPurchaseV2CreateRequestData from a dict
in_app_purchase_v2_create_request_data_from_dict = InAppPurchaseV2CreateRequestData.from_dict(in_app_purchase_v2_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


