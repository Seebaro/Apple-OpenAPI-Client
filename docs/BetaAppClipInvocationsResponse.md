# BetaAppClipInvocationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaAppClipInvocation]**](BetaAppClipInvocation.md) |  | 
**included** | [**List[BetaAppClipInvocationLocalization]**](BetaAppClipInvocationLocalization.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocations_response import BetaAppClipInvocationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationsResponse from a JSON string
beta_app_clip_invocations_response_instance = BetaAppClipInvocationsResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationsResponse.to_json())

# convert the object into a dict
beta_app_clip_invocations_response_dict = beta_app_clip_invocations_response_instance.to_dict()
# create an instance of BetaAppClipInvocationsResponse from a dict
beta_app_clip_invocations_response_from_dict = BetaAppClipInvocationsResponse.from_dict(beta_app_clip_invocations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


