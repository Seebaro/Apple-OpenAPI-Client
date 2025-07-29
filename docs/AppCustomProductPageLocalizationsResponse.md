# AppCustomProductPageLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageLocalization]**](AppCustomProductPageLocalization.md) |  | 
**included** | [**List[AppCustomProductPageLocalizationsResponseIncludedInner]**](AppCustomProductPageLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localizations_response import AppCustomProductPageLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationsResponse from a JSON string
app_custom_product_page_localizations_response_instance = AppCustomProductPageLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationsResponse.to_json())

# convert the object into a dict
app_custom_product_page_localizations_response_dict = app_custom_product_page_localizations_response_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationsResponse from a dict
app_custom_product_page_localizations_response_from_dict = AppCustomProductPageLocalizationsResponse.from_dict(app_custom_product_page_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


