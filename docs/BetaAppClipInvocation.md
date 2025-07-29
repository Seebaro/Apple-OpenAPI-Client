# BetaAppClipInvocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaAppClipInvocationAttributes**](BetaAppClipInvocationAttributes.md) |  | [optional] 
**relationships** | [**BetaAppClipInvocationRelationships**](BetaAppClipInvocationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocation import BetaAppClipInvocation

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocation from a JSON string
beta_app_clip_invocation_instance = BetaAppClipInvocation.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocation.to_json())

# convert the object into a dict
beta_app_clip_invocation_dict = beta_app_clip_invocation_instance.to_dict()
# create an instance of BetaAppClipInvocation from a dict
beta_app_clip_invocation_from_dict = BetaAppClipInvocation.from_dict(beta_app_clip_invocation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


