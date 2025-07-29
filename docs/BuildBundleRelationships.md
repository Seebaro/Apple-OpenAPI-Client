# BuildBundleRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_clip_domain_cache_status** | [**BuildBundleRelationshipsAppClipDomainCacheStatus**](BuildBundleRelationshipsAppClipDomainCacheStatus.md) |  | [optional] 
**app_clip_domain_debug_status** | [**BuildBundleRelationshipsAppClipDomainCacheStatus**](BuildBundleRelationshipsAppClipDomainCacheStatus.md) |  | [optional] 
**beta_app_clip_invocations** | [**BuildBundleRelationshipsBetaAppClipInvocations**](BuildBundleRelationshipsBetaAppClipInvocations.md) |  | [optional] 
**build_bundle_file_sizes** | [**BuildBundleRelationshipsBuildBundleFileSizes**](BuildBundleRelationshipsBuildBundleFileSizes.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_relationships import BuildBundleRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleRelationships from a JSON string
build_bundle_relationships_instance = BuildBundleRelationships.from_json(json)
# print the JSON string representation of the object
print(BuildBundleRelationships.to_json())

# convert the object into a dict
build_bundle_relationships_dict = build_bundle_relationships_instance.to_dict()
# create an instance of BuildBundleRelationships from a dict
build_bundle_relationships_from_dict = BuildBundleRelationships.from_dict(build_bundle_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


