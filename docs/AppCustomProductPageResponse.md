# AppCustomProductPageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPage**](AppCustomProductPage.md) |  | 
**included** | [**List[AppCustomProductPagesResponseIncludedInner]**](AppCustomProductPagesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_response import AppCustomProductPageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageResponse from a JSON string
app_custom_product_page_response_instance = AppCustomProductPageResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageResponse.to_json())

# convert the object into a dict
app_custom_product_page_response_dict = app_custom_product_page_response_instance.to_dict()
# create an instance of AppCustomProductPageResponse from a dict
app_custom_product_page_response_from_dict = AppCustomProductPageResponse.from_dict(app_custom_product_page_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


