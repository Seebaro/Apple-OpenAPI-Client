# BetaAppClipInvocationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaAppClipInvocationCreateRequestData**](BetaAppClipInvocationCreateRequestData.md) |  | 
**included** | [**List[BetaAppClipInvocationLocalizationInlineCreate]**](BetaAppClipInvocationLocalizationInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_create_request import BetaAppClipInvocationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationCreateRequest from a JSON string
beta_app_clip_invocation_create_request_instance = BetaAppClipInvocationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationCreateRequest.to_json())

# convert the object into a dict
beta_app_clip_invocation_create_request_dict = beta_app_clip_invocation_create_request_instance.to_dict()
# create an instance of BetaAppClipInvocationCreateRequest from a dict
beta_app_clip_invocation_create_request_from_dict = BetaAppClipInvocationCreateRequest.from_dict(beta_app_clip_invocation_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


