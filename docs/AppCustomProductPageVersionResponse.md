# AppCustomProductPageVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPageVersion**](AppCustomProductPageVersion.md) |  | 
**included** | [**List[AppCustomProductPageVersionsResponseIncludedInner]**](AppCustomProductPageVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_version_response import AppCustomProductPageVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionResponse from a JSON string
app_custom_product_page_version_response_instance = AppCustomProductPageVersionResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionResponse.to_json())

# convert the object into a dict
app_custom_product_page_version_response_dict = app_custom_product_page_version_response_instance.to_dict()
# create an instance of AppCustomProductPageVersionResponse from a dict
app_custom_product_page_version_response_from_dict = AppCustomProductPageVersionResponse.from_dict(app_custom_product_page_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


