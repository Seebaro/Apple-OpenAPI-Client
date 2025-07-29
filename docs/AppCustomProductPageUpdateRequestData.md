# AppCustomProductPageUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageUpdateRequestDataAttributes**](AppCustomProductPageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_update_request_data import AppCustomProductPageUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageUpdateRequestData from a JSON string
app_custom_product_page_update_request_data_instance = AppCustomProductPageUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageUpdateRequestData.to_json())

# convert the object into a dict
app_custom_product_page_update_request_data_dict = app_custom_product_page_update_request_data_instance.to_dict()
# create an instance of AppCustomProductPageUpdateRequestData from a dict
app_custom_product_page_update_request_data_from_dict = AppCustomProductPageUpdateRequestData.from_dict(app_custom_product_page_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


