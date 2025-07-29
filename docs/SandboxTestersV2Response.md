# SandboxTestersV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SandboxTesterV2]**](SandboxTesterV2.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.sandbox_testers_v2_response import SandboxTestersV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTestersV2Response from a JSON string
sandbox_testers_v2_response_instance = SandboxTestersV2Response.from_json(json)
# print the JSON string representation of the object
print(SandboxTestersV2Response.to_json())

# convert the object into a dict
sandbox_testers_v2_response_dict = sandbox_testers_v2_response_instance.to_dict()
# create an instance of SandboxTestersV2Response from a dict
sandbox_testers_v2_response_from_dict = SandboxTestersV2Response.from_dict(sandbox_testers_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


