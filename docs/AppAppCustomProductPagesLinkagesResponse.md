# AppAppCustomProductPagesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageVersionRelationshipsAppCustomProductPageData]**](AppCustomProductPageVersionRelationshipsAppCustomProductPageData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_custom_product_pages_linkages_response import AppAppCustomProductPagesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppCustomProductPagesLinkagesResponse from a JSON string
app_app_custom_product_pages_linkages_response_instance = AppAppCustomProductPagesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppCustomProductPagesLinkagesResponse.to_json())

# convert the object into a dict
app_app_custom_product_pages_linkages_response_dict = app_app_custom_product_pages_linkages_response_instance.to_dict()
# create an instance of AppAppCustomProductPagesLinkagesResponse from a dict
app_app_custom_product_pages_linkages_response_from_dict = AppAppCustomProductPagesLinkagesResponse.from_dict(app_app_custom_product_pages_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


