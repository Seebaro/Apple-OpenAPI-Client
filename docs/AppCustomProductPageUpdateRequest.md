# AppCustomProductPageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPageUpdateRequestData**](AppCustomProductPageUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_update_request import AppCustomProductPageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageUpdateRequest from a JSON string
app_custom_product_page_update_request_instance = AppCustomProductPageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageUpdateRequest.to_json())

# convert the object into a dict
app_custom_product_page_update_request_dict = app_custom_product_page_update_request_instance.to_dict()
# create an instance of AppCustomProductPageUpdateRequest from a dict
app_custom_product_page_update_request_from_dict = AppCustomProductPageUpdateRequest.from_dict(app_custom_product_page_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


