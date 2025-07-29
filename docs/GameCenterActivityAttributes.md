# GameCenterActivityAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 
**play_style** | **str** |  | [optional] 
**minimum_players_count** | **int** |  | [optional] 
**maximum_players_count** | **int** |  | [optional] 
**supports_party_code** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_attributes import GameCenterActivityAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityAttributes from a JSON string
game_center_activity_attributes_instance = GameCenterActivityAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityAttributes.to_json())

# convert the object into a dict
game_center_activity_attributes_dict = game_center_activity_attributes_instance.to_dict()
# create an instance of GameCenterActivityAttributes from a dict
game_center_activity_attributes_from_dict = GameCenterActivityAttributes.from_dict(game_center_activity_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


