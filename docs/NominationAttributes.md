# NominationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**last_modified_date** | **datetime** |  | [optional] 
**submitted_date** | **datetime** |  | [optional] 
**state** | **str** |  | [optional] 
**publish_start_date** | **datetime** |  | [optional] 
**publish_end_date** | **datetime** |  | [optional] 
**device_families** | [**List[DeviceFamily]**](DeviceFamily.md) |  | [optional] 
**locales** | **List[str]** |  | [optional] 
**supplemental_materials_uris** | **List[str]** |  | [optional] 
**has_in_app_events** | **bool** |  | [optional] 
**launch_in_select_markets_first** | **bool** |  | [optional] 
**notes** | **str** |  | [optional] 
**pre_order_enabled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.nomination_attributes import NominationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of NominationAttributes from a JSON string
nomination_attributes_instance = NominationAttributes.from_json(json)
# print the JSON string representation of the object
print(NominationAttributes.to_json())

# convert the object into a dict
nomination_attributes_dict = nomination_attributes_instance.to_dict()
# create an instance of NominationAttributes from a dict
nomination_attributes_from_dict = NominationAttributes.from_dict(nomination_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


