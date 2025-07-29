# AppCustomProductPageRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**app_custom_product_page_versions** | [**AppCustomProductPageRelationshipsAppCustomProductPageVersions**](AppCustomProductPageRelationshipsAppCustomProductPageVersions.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_relationships import AppCustomProductPageRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageRelationships from a JSON string
app_custom_product_page_relationships_instance = AppCustomProductPageRelationships.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageRelationships.to_json())

# convert the object into a dict
app_custom_product_page_relationships_dict = app_custom_product_page_relationships_instance.to_dict()
# create an instance of AppCustomProductPageRelationships from a dict
app_custom_product_page_relationships_from_dict = AppCustomProductPageRelationships.from_dict(app_custom_product_page_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


