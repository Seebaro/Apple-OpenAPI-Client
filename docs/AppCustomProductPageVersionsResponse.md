# AppCustomProductPageVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageVersion]**](AppCustomProductPageVersion.md) |  | 
**included** | [**List[AppCustomProductPageVersionsResponseIncludedInner]**](AppCustomProductPageVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_versions_response import AppCustomProductPageVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionsResponse from a JSON string
app_custom_product_page_versions_response_instance = AppCustomProductPageVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionsResponse.to_json())

# convert the object into a dict
app_custom_product_page_versions_response_dict = app_custom_product_page_versions_response_instance.to_dict()
# create an instance of AppCustomProductPageVersionsResponse from a dict
app_custom_product_page_versions_response_from_dict = AppCustomProductPageVersionsResponse.from_dict(app_custom_product_page_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


