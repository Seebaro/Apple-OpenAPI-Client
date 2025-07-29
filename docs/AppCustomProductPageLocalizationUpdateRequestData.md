# AppCustomProductPageLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageLocalizationUpdateRequestDataAttributes**](AppCustomProductPageLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localization_update_request_data import AppCustomProductPageLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationUpdateRequestData from a JSON string
app_custom_product_page_localization_update_request_data_instance = AppCustomProductPageLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationUpdateRequestData.to_json())

# convert the object into a dict
app_custom_product_page_localization_update_request_data_dict = app_custom_product_page_localization_update_request_data_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationUpdateRequestData from a dict
app_custom_product_page_localization_update_request_data_from_dict = AppCustomProductPageLocalizationUpdateRequestData.from_dict(app_custom_product_page_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


