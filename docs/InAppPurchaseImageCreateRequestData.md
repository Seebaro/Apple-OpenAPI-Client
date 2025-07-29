# InAppPurchaseImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**InAppPurchaseImageCreateRequestDataRelationships**](InAppPurchaseImageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_image_create_request_data import InAppPurchaseImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImageCreateRequestData from a JSON string
in_app_purchase_image_create_request_data_instance = InAppPurchaseImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImageCreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_image_create_request_data_dict = in_app_purchase_image_create_request_data_instance.to_dict()
# create an instance of InAppPurchaseImageCreateRequestData from a dict
in_app_purchase_image_create_request_data_from_dict = InAppPurchaseImageCreateRequestData.from_dict(in_app_purchase_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


