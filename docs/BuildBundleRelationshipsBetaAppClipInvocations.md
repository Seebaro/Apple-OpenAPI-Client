# BuildBundleRelationshipsBetaAppClipInvocations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[BetaAppClipInvocationLocalizationInlineCreateRelationshipsBetaAppClipInvocationData]**](BetaAppClipInvocationLocalizationInlineCreateRelationshipsBetaAppClipInvocationData.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_relationships_beta_app_clip_invocations import BuildBundleRelationshipsBetaAppClipInvocations

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleRelationshipsBetaAppClipInvocations from a JSON string
build_bundle_relationships_beta_app_clip_invocations_instance = BuildBundleRelationshipsBetaAppClipInvocations.from_json(json)
# print the JSON string representation of the object
print(BuildBundleRelationshipsBetaAppClipInvocations.to_json())

# convert the object into a dict
build_bundle_relationships_beta_app_clip_invocations_dict = build_bundle_relationships_beta_app_clip_invocations_instance.to_dict()
# create an instance of BuildBundleRelationshipsBetaAppClipInvocations from a dict
build_bundle_relationships_beta_app_clip_invocations_from_dict = BuildBundleRelationshipsBetaAppClipInvocations.from_dict(build_bundle_relationships_beta_app_clip_invocations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


