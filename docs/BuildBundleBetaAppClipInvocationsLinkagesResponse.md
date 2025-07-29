# BuildBundleBetaAppClipInvocationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaAppClipInvocationLocalizationInlineCreateRelationshipsBetaAppClipInvocationData]**](BetaAppClipInvocationLocalizationInlineCreateRelationshipsBetaAppClipInvocationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_beta_app_clip_invocations_linkages_response import BuildBundleBetaAppClipInvocationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleBetaAppClipInvocationsLinkagesResponse from a JSON string
build_bundle_beta_app_clip_invocations_linkages_response_instance = BuildBundleBetaAppClipInvocationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildBundleBetaAppClipInvocationsLinkagesResponse.to_json())

# convert the object into a dict
build_bundle_beta_app_clip_invocations_linkages_response_dict = build_bundle_beta_app_clip_invocations_linkages_response_instance.to_dict()
# create an instance of BuildBundleBetaAppClipInvocationsLinkagesResponse from a dict
build_bundle_beta_app_clip_invocations_linkages_response_from_dict = BuildBundleBetaAppClipInvocationsLinkagesResponse.from_dict(build_bundle_beta_app_clip_invocations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


