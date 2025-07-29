# GameCenterMatchmakingTeamAssignment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**player_id** | **str** |  | [optional] 
**team** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_team_assignment import GameCenterMatchmakingTeamAssignment

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTeamAssignment from a JSON string
game_center_matchmaking_team_assignment_instance = GameCenterMatchmakingTeamAssignment.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTeamAssignment.to_json())

# convert the object into a dict
game_center_matchmaking_team_assignment_dict = game_center_matchmaking_team_assignment_instance.to_dict()
# create an instance of GameCenterMatchmakingTeamAssignment from a dict
game_center_matchmaking_team_assignment_from_dict = GameCenterMatchmakingTeamAssignment.from_dict(game_center_matchmaking_team_assignment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


