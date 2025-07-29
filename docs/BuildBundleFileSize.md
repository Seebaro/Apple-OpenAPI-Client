# BuildBundleFileSize


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BuildBundleFileSizeAttributes**](BuildBundleFileSizeAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_file_size import BuildBundleFileSize

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleFileSize from a JSON string
build_bundle_file_size_instance = BuildBundleFileSize.from_json(json)
# print the JSON string representation of the object
print(BuildBundleFileSize.to_json())

# convert the object into a dict
build_bundle_file_size_dict = build_bundle_file_size_instance.to_dict()
# create an instance of BuildBundleFileSize from a dict
build_bundle_file_size_from_dict = BuildBundleFileSize.from_dict(build_bundle_file_size_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


