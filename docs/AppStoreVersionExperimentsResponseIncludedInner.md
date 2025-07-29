# AppStoreVersionExperimentsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentAttributes**](AppStoreVersionExperimentTreatmentAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentTreatmentRelationships**](AppStoreVersionExperimentTreatmentRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiments_response_included_inner import AppStoreVersionExperimentsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentsResponseIncludedInner from a JSON string
app_store_version_experiments_response_included_inner_instance = AppStoreVersionExperimentsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentsResponseIncludedInner.to_json())

# convert the object into a dict
app_store_version_experiments_response_included_inner_dict = app_store_version_experiments_response_included_inner_instance.to_dict()
# create an instance of AppStoreVersionExperimentsResponseIncludedInner from a dict
app_store_version_experiments_response_included_inner_from_dict = AppStoreVersionExperimentsResponseIncludedInner.from_dict(app_store_version_experiments_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


