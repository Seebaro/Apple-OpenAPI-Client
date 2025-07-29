# CiArtifactAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_type** | **str** |  | [optional] 
**file_name** | **str** |  | [optional] 
**file_size** | **int** |  | [optional] 
**download_url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_artifact_attributes import CiArtifactAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiArtifactAttributes from a JSON string
ci_artifact_attributes_instance = CiArtifactAttributes.from_json(json)
# print the JSON string representation of the object
print(CiArtifactAttributes.to_json())

# convert the object into a dict
ci_artifact_attributes_dict = ci_artifact_attributes_instance.to_dict()
# create an instance of CiArtifactAttributes from a dict
ci_artifact_attributes_from_dict = CiArtifactAttributes.from_dict(ci_artifact_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


