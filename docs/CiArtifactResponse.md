# CiArtifactResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiArtifact**](CiArtifact.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_artifact_response import CiArtifactResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiArtifactResponse from a JSON string
ci_artifact_response_instance = CiArtifactResponse.from_json(json)
# print the JSON string representation of the object
print(CiArtifactResponse.to_json())

# convert the object into a dict
ci_artifact_response_dict = ci_artifact_response_instance.to_dict()
# create an instance of CiArtifactResponse from a dict
ci_artifact_response_from_dict = CiArtifactResponse.from_dict(ci_artifact_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


