# BuildAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | [optional] 
**uploaded_date** | **datetime** |  | [optional] 
**expiration_date** | **datetime** |  | [optional] 
**expired** | **bool** |  | [optional] 
**min_os_version** | **str** |  | [optional] 
**ls_minimum_system_version** | **str** |  | [optional] 
**computed_min_mac_os_version** | **str** |  | [optional] 
**computed_min_vision_os_version** | **str** |  | [optional] 
**icon_asset_token** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**processing_state** | **str** |  | [optional] 
**build_audience_type** | [**BuildAudienceType**](BuildAudienceType.md) |  | [optional] 
**uses_non_exempt_encryption** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.build_attributes import BuildAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BuildAttributes from a JSON string
build_attributes_instance = BuildAttributes.from_json(json)
# print the JSON string representation of the object
print(BuildAttributes.to_json())

# convert the object into a dict
build_attributes_dict = build_attributes_instance.to_dict()
# create an instance of BuildAttributes from a dict
build_attributes_from_dict = BuildAttributes.from_dict(build_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


