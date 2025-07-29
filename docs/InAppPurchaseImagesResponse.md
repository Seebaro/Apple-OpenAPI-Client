# InAppPurchaseImagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchaseImage]**](InAppPurchaseImage.md) |  | 
**included** | [**List[InAppPurchaseV2]**](InAppPurchaseV2.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_images_response import InAppPurchaseImagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImagesResponse from a JSON string
in_app_purchase_images_response_instance = InAppPurchaseImagesResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImagesResponse.to_json())

# convert the object into a dict
in_app_purchase_images_response_dict = in_app_purchase_images_response_instance.to_dict()
# create an instance of InAppPurchaseImagesResponse from a dict
in_app_purchase_images_response_from_dict = InAppPurchaseImagesResponse.from_dict(in_app_purchase_images_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


