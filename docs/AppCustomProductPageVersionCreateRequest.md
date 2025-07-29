# AppCustomProductPageVersionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPageVersionCreateRequestData**](AppCustomProductPageVersionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_version_create_request import AppCustomProductPageVersionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionCreateRequest from a JSON string
app_custom_product_page_version_create_request_instance = AppCustomProductPageVersionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionCreateRequest.to_json())

# convert the object into a dict
app_custom_product_page_version_create_request_dict = app_custom_product_page_version_create_request_instance.to_dict()
# create an instance of AppCustomProductPageVersionCreateRequest from a dict
app_custom_product_page_version_create_request_from_dict = AppCustomProductPageVersionCreateRequest.from_dict(app_custom_product_page_version_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


