# BetaAppClipInvocationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaAppClipInvocation**](BetaAppClipInvocation.md) |  | 
**included** | [**List[BetaAppClipInvocationLocalization]**](BetaAppClipInvocationLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_response import BetaAppClipInvocationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationResponse from a JSON string
beta_app_clip_invocation_response_instance = BetaAppClipInvocationResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationResponse.to_json())

# convert the object into a dict
beta_app_clip_invocation_response_dict = beta_app_clip_invocation_response_instance.to_dict()
# create an instance of BetaAppClipInvocationResponse from a dict
beta_app_clip_invocation_response_from_dict = BetaAppClipInvocationResponse.from_dict(beta_app_clip_invocation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


