# GameCenterMatchmakingTeamAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**min_players** | **int** |  | [optional] 
**max_players** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_team_attributes import GameCenterMatchmakingTeamAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTeamAttributes from a JSON string
game_center_matchmaking_team_attributes_instance = GameCenterMatchmakingTeamAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTeamAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_team_attributes_dict = game_center_matchmaking_team_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingTeamAttributes from a dict
game_center_matchmaking_team_attributes_from_dict = GameCenterMatchmakingTeamAttributes.from_dict(game_center_matchmaking_team_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


