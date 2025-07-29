# AppCiProductLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsCiProductData**](AppRelationshipsCiProductData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_ci_product_linkage_response import AppCiProductLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCiProductLinkageResponse from a JSON string
app_ci_product_linkage_response_instance = AppCiProductLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppCiProductLinkageResponse.to_json())

# convert the object into a dict
app_ci_product_linkage_response_dict = app_ci_product_linkage_response_instance.to_dict()
# create an instance of AppCiProductLinkageResponse from a dict
app_ci_product_linkage_response_from_dict = AppCiProductLinkageResponse.from_dict(app_ci_product_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


