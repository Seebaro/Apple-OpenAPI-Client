# InAppPurchaseContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseContentAttributes**](InAppPurchaseContentAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotRelationships**](InAppPurchaseAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_content import InAppPurchaseContent

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseContent from a JSON string
in_app_purchase_content_instance = InAppPurchaseContent.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseContent.to_json())

# convert the object into a dict
in_app_purchase_content_dict = in_app_purchase_content_instance.to_dict()
# create an instance of InAppPurchaseContent from a dict
in_app_purchase_content_from_dict = InAppPurchaseContent.from_dict(in_app_purchase_content_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


