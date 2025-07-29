# InAppPurchaseImage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseImageAttributes**](InAppPurchaseImageAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseImageRelationships**](InAppPurchaseImageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_image import InAppPurchaseImage

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImage from a JSON string
in_app_purchase_image_instance = InAppPurchaseImage.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImage.to_json())

# convert the object into a dict
in_app_purchase_image_dict = in_app_purchase_image_instance.to_dict()
# create an instance of InAppPurchaseImage from a dict
in_app_purchase_image_from_dict = InAppPurchaseImage.from_dict(in_app_purchase_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


