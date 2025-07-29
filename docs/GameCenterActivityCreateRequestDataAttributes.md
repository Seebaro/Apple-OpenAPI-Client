# GameCenterActivityCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**vendor_identifier** | **str** |  | 
**play_style** | **str** |  | [optional] 
**minimum_players_count** | **int** |  | [optional] 
**maximum_players_count** | **int** |  | [optional] 
**supports_party_code** | **bool** |  | [optional] 
**properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_create_request_data_attributes import GameCenterActivityCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityCreateRequestDataAttributes from a JSON string
game_center_activity_create_request_data_attributes_instance = GameCenterActivityCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_activity_create_request_data_attributes_dict = game_center_activity_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterActivityCreateRequestDataAttributes from a dict
game_center_activity_create_request_data_attributes_from_dict = GameCenterActivityCreateRequestDataAttributes.from_dict(game_center_activity_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


