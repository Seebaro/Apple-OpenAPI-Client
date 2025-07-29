# AppCustomProductPageLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPageLocalization**](AppCustomProductPageLocalization.md) |  | 
**included** | [**List[AppCustomProductPageLocalizationsResponseIncludedInner]**](AppCustomProductPageLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_localization_response import AppCustomProductPageLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationResponse from a JSON string
app_custom_product_page_localization_response_instance = AppCustomProductPageLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationResponse.to_json())

# convert the object into a dict
app_custom_product_page_localization_response_dict = app_custom_product_page_localization_response_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationResponse from a dict
app_custom_product_page_localization_response_from_dict = AppCustomProductPageLocalizationResponse.from_dict(app_custom_product_page_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


