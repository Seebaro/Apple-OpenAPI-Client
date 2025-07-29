# NominationCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**type** | **str** |  | 
**description** | **str** |  | 
**submitted** | **bool** |  | 
**publish_start_date** | **datetime** |  | 
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
from openapi_client.models.nomination_create_request_data_attributes import NominationCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of NominationCreateRequestDataAttributes from a JSON string
nomination_create_request_data_attributes_instance = NominationCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(NominationCreateRequestDataAttributes.to_json())

# convert the object into a dict
nomination_create_request_data_attributes_dict = nomination_create_request_data_attributes_instance.to_dict()
# create an instance of NominationCreateRequestDataAttributes from a dict
nomination_create_request_data_attributes_from_dict = NominationCreateRequestDataAttributes.from_dict(nomination_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


