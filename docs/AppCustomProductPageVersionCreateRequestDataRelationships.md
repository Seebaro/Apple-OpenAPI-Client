# AppCustomProductPageVersionCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_custom_product_page** | [**AppCustomProductPageVersionCreateRequestDataRelationshipsAppCustomProductPage**](AppCustomProductPageVersionCreateRequestDataRelationshipsAppCustomProductPage.md) |  | 
**app_custom_product_page_localizations** | [**AppCustomProductPageVersionInlineCreateRelationshipsAppCustomProductPageLocalizations**](AppCustomProductPageVersionInlineCreateRelationshipsAppCustomProductPageLocalizations.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_version_create_request_data_relationships import AppCustomProductPageVersionCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionCreateRequestDataRelationships from a JSON string
app_custom_product_page_version_create_request_data_relationships_instance = AppCustomProductPageVersionCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionCreateRequestDataRelationships.to_json())

# convert the object into a dict
app_custom_product_page_version_create_request_data_relationships_dict = app_custom_product_page_version_create_request_data_relationships_instance.to_dict()
# create an instance of AppCustomProductPageVersionCreateRequestDataRelationships from a dict
app_custom_product_page_version_create_request_data_relationships_from_dict = AppCustomProductPageVersionCreateRequestDataRelationships.from_dict(app_custom_product_page_version_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


