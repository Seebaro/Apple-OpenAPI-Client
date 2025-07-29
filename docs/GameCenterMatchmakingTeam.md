# GameCenterMatchmakingTeam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingTeamAttributes**](GameCenterMatchmakingTeamAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_team import GameCenterMatchmakingTeam

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTeam from a JSON string
game_center_matchmaking_team_instance = GameCenterMatchmakingTeam.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTeam.to_json())

# convert the object into a dict
game_center_matchmaking_team_dict = game_center_matchmaking_team_instance.to_dict()
# create an instance of GameCenterMatchmakingTeam from a dict
game_center_matchmaking_team_from_dict = GameCenterMatchmakingTeam.from_dict(game_center_matchmaking_team_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


