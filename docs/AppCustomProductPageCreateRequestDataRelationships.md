# AppCustomProductPageCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AccessibilityDeclarationCreateRequestDataRelationshipsApp**](AccessibilityDeclarationCreateRequestDataRelationshipsApp.md) |  | 
**app_custom_product_page_versions** | [**AppCustomProductPageCreateRequestDataRelationshipsAppCustomProductPageVersions**](AppCustomProductPageCreateRequestDataRelationshipsAppCustomProductPageVersions.md) |  | [optional] 
**app_store_version_template** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**custom_product_page_template** | [**AppCustomProductPageVersionRelationshipsAppCustomProductPage**](AppCustomProductPageVersionRelationshipsAppCustomProductPage.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_create_request_data_relationships import AppCustomProductPageCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageCreateRequestDataRelationships from a JSON string
app_custom_product_page_create_request_data_relationships_instance = AppCustomProductPageCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageCreateRequestDataRelationships.to_json())

# convert the object into a dict
app_custom_product_page_create_request_data_relationships_dict = app_custom_product_page_create_request_data_relationships_instance.to_dict()
# create an instance of AppCustomProductPageCreateRequestDataRelationships from a dict
app_custom_product_page_create_request_data_relationships_from_dict = AppCustomProductPageCreateRequestDataRelationships.from_dict(app_custom_product_page_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


