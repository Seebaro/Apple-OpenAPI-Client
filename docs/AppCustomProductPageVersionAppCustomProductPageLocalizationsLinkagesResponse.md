# AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageVersionRelationshipsAppCustomProductPageLocalizationsDataInner]**](AppCustomProductPageVersionRelationshipsAppCustomProductPageLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_version_app_custom_product_page_localizations_linkages_response import AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse from a JSON string
app_custom_product_page_version_app_custom_product_page_localizations_linkages_response_instance = AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
app_custom_product_page_version_app_custom_product_page_localizations_linkages_response_dict = app_custom_product_page_version_app_custom_product_page_localizations_linkages_response_instance.to_dict()
# create an instance of AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse from a dict
app_custom_product_page_version_app_custom_product_page_localizations_linkages_response_from_dict = AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.from_dict(app_custom_product_page_version_app_custom_product_page_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


