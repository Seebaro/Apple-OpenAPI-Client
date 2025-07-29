# GameCenterMatchmakingTeamResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterMatchmakingTeam**](GameCenterMatchmakingTeam.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_team_response import GameCenterMatchmakingTeamResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTeamResponse from a JSON string
game_center_matchmaking_team_response_instance = GameCenterMatchmakingTeamResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTeamResponse.to_json())

# convert the object into a dict
game_center_matchmaking_team_response_dict = game_center_matchmaking_team_response_instance.to_dict()
# create an instance of GameCenterMatchmakingTeamResponse from a dict
game_center_matchmaking_team_response_from_dict = GameCenterMatchmakingTeamResponse.from_dict(game_center_matchmaking_team_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


