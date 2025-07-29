# GameCenterMatchmakingTeamCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**min_players** | **int** |  | 
**max_players** | **int** |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_team_create_request_data_attributes import GameCenterMatchmakingTeamCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTeamCreateRequestDataAttributes from a JSON string
game_center_matchmaking_team_create_request_data_attributes_instance = GameCenterMatchmakingTeamCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTeamCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_team_create_request_data_attributes_dict = game_center_matchmaking_team_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingTeamCreateRequestDataAttributes from a dict
game_center_matchmaking_team_create_request_data_attributes_from_dict = GameCenterMatchmakingTeamCreateRequestDataAttributes.from_dict(game_center_matchmaking_team_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


