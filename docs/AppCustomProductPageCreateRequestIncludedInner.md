# AppCustomProductPageCreateRequestIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**AppCustomProductPageVersionInlineCreateAttributes**](AppCustomProductPageVersionInlineCreateAttributes.md) |  | 
**relationships** | [**AppCustomProductPageVersionInlineCreateRelationships**](AppCustomProductPageVersionInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_create_request_included_inner import AppCustomProductPageCreateRequestIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageCreateRequestIncludedInner from a JSON string
app_custom_product_page_create_request_included_inner_instance = AppCustomProductPageCreateRequestIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageCreateRequestIncludedInner.to_json())

# convert the object into a dict
app_custom_product_page_create_request_included_inner_dict = app_custom_product_page_create_request_included_inner_instance.to_dict()
# create an instance of AppCustomProductPageCreateRequestIncludedInner from a dict
app_custom_product_page_create_request_included_inner_from_dict = AppCustomProductPageCreateRequestIncludedInner.from_dict(app_custom_product_page_create_request_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


