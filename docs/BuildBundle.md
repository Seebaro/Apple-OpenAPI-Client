# BuildBundle


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BuildBundleAttributes**](BuildBundleAttributes.md) |  | [optional] 
**relationships** | [**BuildBundleRelationships**](BuildBundleRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle import BuildBundle

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundle from a JSON string
build_bundle_instance = BuildBundle.from_json(json)
# print the JSON string representation of the object
print(BuildBundle.to_json())

# convert the object into a dict
build_bundle_dict = build_bundle_instance.to_dict()
# create an instance of BuildBundle from a dict
build_bundle_from_dict = BuildBundle.from_dict(build_bundle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


