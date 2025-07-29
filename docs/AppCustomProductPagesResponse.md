# AppCustomProductPagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPage]**](AppCustomProductPage.md) |  | 
**included** | [**List[AppCustomProductPagesResponseIncludedInner]**](AppCustomProductPagesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_pages_response import AppCustomProductPagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPagesResponse from a JSON string
app_custom_product_pages_response_instance = AppCustomProductPagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPagesResponse.to_json())

# convert the object into a dict
app_custom_product_pages_response_dict = app_custom_product_pages_response_instance.to_dict()
# create an instance of AppCustomProductPagesResponse from a dict
app_custom_product_pages_response_from_dict = AppCustomProductPagesResponse.from_dict(app_custom_product_pages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


