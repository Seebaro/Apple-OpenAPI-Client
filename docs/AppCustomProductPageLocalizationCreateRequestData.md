# AppCustomProductPageLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppCustomProductPageLocalizationInlineCreateAttributes**](AppCustomProductPageLocalizationInlineCreateAttributes.md) |  | 
**relationships** | [**AppCustomProductPageLocalizationCreateRequestDataRelationships**](AppCustomProductPageLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_localization_create_request_data import AppCustomProductPageLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationCreateRequestData from a JSON string
app_custom_product_page_localization_create_request_data_instance = AppCustomProductPageLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationCreateRequestData.to_json())

# convert the object into a dict
app_custom_product_page_localization_create_request_data_dict = app_custom_product_page_localization_create_request_data_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationCreateRequestData from a dict
app_custom_product_page_localization_create_request_data_from_dict = AppCustomProductPageLocalizationCreateRequestData.from_dict(app_custom_product_page_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


