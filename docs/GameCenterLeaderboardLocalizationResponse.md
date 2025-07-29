# GameCenterLeaderboardLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardLocalization**](GameCenterLeaderboardLocalization.md) |  | 
**included** | [**List[GameCenterLeaderboardLocalizationsResponseIncludedInner]**](GameCenterLeaderboardLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_localization_response import GameCenterLeaderboardLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardLocalizationResponse from a JSON string
game_center_leaderboard_localization_response_instance = GameCenterLeaderboardLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardLocalizationResponse.to_json())

# convert the object into a dict
game_center_leaderboard_localization_response_dict = game_center_leaderboard_localization_response_instance.to_dict()
# create an instance of GameCenterLeaderboardLocalizationResponse from a dict
game_center_leaderboard_localization_response_from_dict = GameCenterLeaderboardLocalizationResponse.from_dict(game_center_leaderboard_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


