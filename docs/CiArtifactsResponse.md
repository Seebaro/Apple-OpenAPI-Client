# CiArtifactsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiArtifact]**](CiArtifact.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_artifacts_response import CiArtifactsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiArtifactsResponse from a JSON string
ci_artifacts_response_instance = CiArtifactsResponse.from_json(json)
# print the JSON string representation of the object
print(CiArtifactsResponse.to_json())

# convert the object into a dict
ci_artifacts_response_dict = ci_artifacts_response_instance.to_dict()
# create an instance of CiArtifactsResponse from a dict
ci_artifacts_response_from_dict = CiArtifactsResponse.from_dict(ci_artifacts_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


