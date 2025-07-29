# GameCenterActivityUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**play_style** | **str** |  | [optional] 
**minimum_players_count** | **int** |  | [optional] 
**maximum_players_count** | **int** |  | [optional] 
**supports_party_code** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_update_request_data_attributes import GameCenterActivityUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityUpdateRequestDataAttributes from a JSON string
game_center_activity_update_request_data_attributes_instance = GameCenterActivityUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityUpdateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_activity_update_request_data_attributes_dict = game_center_activity_update_request_data_attributes_instance.to_dict()
# create an instance of GameCenterActivityUpdateRequestDataAttributes from a dict
game_center_activity_update_request_data_attributes_from_dict = GameCenterActivityUpdateRequestDataAttributes.from_dict(game_center_activity_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


