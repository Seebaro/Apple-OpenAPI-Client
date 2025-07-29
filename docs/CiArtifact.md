# CiArtifact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiArtifactAttributes**](CiArtifactAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_artifact import CiArtifact

# TODO update the JSON string below
json = "{}"
# create an instance of CiArtifact from a JSON string
ci_artifact_instance = CiArtifact.from_json(json)
# print the JSON string representation of the object
print(CiArtifact.to_json())

# convert the object into a dict
ci_artifact_dict = ci_artifact_instance.to_dict()
# create an instance of CiArtifact from a dict
ci_artifact_from_dict = CiArtifact.from_dict(ci_artifact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


