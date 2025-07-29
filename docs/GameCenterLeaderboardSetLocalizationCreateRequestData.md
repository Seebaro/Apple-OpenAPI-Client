# GameCenterLeaderboardSetLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetLocalizationCreateRequestDataAttributes**](GameCenterLeaderboardSetLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterLeaderboardSetLocalizationCreateRequestDataRelationships**](GameCenterLeaderboardSetLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_localization_create_request_data import GameCenterLeaderboardSetLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetLocalizationCreateRequestData from a JSON string
game_center_leaderboard_set_localization_create_request_data_instance = GameCenterLeaderboardSetLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetLocalizationCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_set_localization_create_request_data_dict = game_center_leaderboard_set_localization_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardSetLocalizationCreateRequestData from a dict
game_center_leaderboard_set_localization_create_request_data_from_dict = GameCenterLeaderboardSetLocalizationCreateRequestData.from_dict(game_center_leaderboard_set_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


