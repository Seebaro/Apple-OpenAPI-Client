# AppStoreVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentV2Attributes**](AppStoreVersionExperimentV2Attributes.md) |  | [optional] 
**relationships** | [**AlternativeDistributionPackageRelationships**](AlternativeDistributionPackageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_versions_response_included_inner import AppStoreVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionsResponseIncludedInner from a JSON string
app_store_versions_response_included_inner_instance = AppStoreVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionsResponseIncludedInner.to_json())

# convert the object into a dict
app_store_versions_response_included_inner_dict = app_store_versions_response_included_inner_instance.to_dict()
# create an instance of AppStoreVersionsResponseIncludedInner from a dict
app_store_versions_response_included_inner_from_dict = AppStoreVersionsResponseIncludedInner.from_dict(app_store_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


