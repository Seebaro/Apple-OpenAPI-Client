# AppCustomProductPageVersionUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageVersionInlineCreateAttributes**](AppCustomProductPageVersionInlineCreateAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_version_update_request_data import AppCustomProductPageVersionUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionUpdateRequestData from a JSON string
app_custom_product_page_version_update_request_data_instance = AppCustomProductPageVersionUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionUpdateRequestData.to_json())

# convert the object into a dict
app_custom_product_page_version_update_request_data_dict = app_custom_product_page_version_update_request_data_instance.to_dict()
# create an instance of AppCustomProductPageVersionUpdateRequestData from a dict
app_custom_product_page_version_update_request_data_from_dict = AppCustomProductPageVersionUpdateRequestData.from_dict(app_custom_product_page_version_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


