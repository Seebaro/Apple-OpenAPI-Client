# BuildBundleRelationshipsBuildBundleFileSizes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[BuildBundleRelationshipsBuildBundleFileSizesDataInner]**](BuildBundleRelationshipsBuildBundleFileSizesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_relationships_build_bundle_file_sizes import BuildBundleRelationshipsBuildBundleFileSizes

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleRelationshipsBuildBundleFileSizes from a JSON string
build_bundle_relationships_build_bundle_file_sizes_instance = BuildBundleRelationshipsBuildBundleFileSizes.from_json(json)
# print the JSON string representation of the object
print(BuildBundleRelationshipsBuildBundleFileSizes.to_json())

# convert the object into a dict
build_bundle_relationships_build_bundle_file_sizes_dict = build_bundle_relationships_build_bundle_file_sizes_instance.to_dict()
# create an instance of BuildBundleRelationshipsBuildBundleFileSizes from a dict
build_bundle_relationships_build_bundle_file_sizes_from_dict = BuildBundleRelationshipsBuildBundleFileSizes.from_dict(build_bundle_relationships_build_bundle_file_sizes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


