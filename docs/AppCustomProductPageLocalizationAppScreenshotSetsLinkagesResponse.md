# AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageLocalizationRelationshipsAppScreenshotSetsDataInner]**](AppCustomProductPageLocalizationRelationshipsAppScreenshotSetsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localization_app_screenshot_sets_linkages_response import AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse from a JSON string
app_custom_product_page_localization_app_screenshot_sets_linkages_response_instance = AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse.to_json())

# convert the object into a dict
app_custom_product_page_localization_app_screenshot_sets_linkages_response_dict = app_custom_product_page_localization_app_screenshot_sets_linkages_response_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse from a dict
app_custom_product_page_localization_app_screenshot_sets_linkages_response_from_dict = AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse.from_dict(app_custom_product_page_localization_app_screenshot_sets_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


