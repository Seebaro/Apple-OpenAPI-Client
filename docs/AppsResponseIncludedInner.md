# AppsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentV2Attributes**](AppStoreVersionExperimentV2Attributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentV2Relationships**](AppStoreVersionExperimentV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.apps_response_included_inner import AppsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppsResponseIncludedInner from a JSON string
apps_response_included_inner_instance = AppsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppsResponseIncludedInner.to_json())

# convert the object into a dict
apps_response_included_inner_dict = apps_response_included_inner_instance.to_dict()
# create an instance of AppsResponseIncludedInner from a dict
apps_response_included_inner_from_dict = AppsResponseIncludedInner.from_dict(apps_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


