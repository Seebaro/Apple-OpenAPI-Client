# AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersionData]**](AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersionData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_app_custom_product_page_versions_linkages_response import AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse from a JSON string
app_custom_product_page_app_custom_product_page_versions_linkages_response_instance = AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.to_json())

# convert the object into a dict
app_custom_product_page_app_custom_product_page_versions_linkages_response_dict = app_custom_product_page_app_custom_product_page_versions_linkages_response_instance.to_dict()
# create an instance of AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse from a dict
app_custom_product_page_app_custom_product_page_versions_linkages_response_from_dict = AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.from_dict(app_custom_product_page_app_custom_product_page_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


