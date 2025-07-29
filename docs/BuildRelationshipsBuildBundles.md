# BuildRelationshipsBuildBundles


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[BetaAppClipInvocationCreateRequestDataRelationshipsBuildBundleData]**](BetaAppClipInvocationCreateRequestDataRelationshipsBuildBundleData.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_relationships_build_bundles import BuildRelationshipsBuildBundles

# TODO update the JSON string below
json = "{}"
# create an instance of BuildRelationshipsBuildBundles from a JSON string
build_relationships_build_bundles_instance = BuildRelationshipsBuildBundles.from_json(json)
# print the JSON string representation of the object
print(BuildRelationshipsBuildBundles.to_json())

# convert the object into a dict
build_relationships_build_bundles_dict = build_relationships_build_bundles_instance.to_dict()
# create an instance of BuildRelationshipsBuildBundles from a dict
build_relationships_build_bundles_from_dict = BuildRelationshipsBuildBundles.from_dict(build_relationships_build_bundles_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


