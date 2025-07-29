# GameCenterLeaderboardSetCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetCreateRequestDataAttributes**](GameCenterLeaderboardSetCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterLeaderboardSetCreateRequestDataRelationships**](GameCenterLeaderboardSetCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_create_request_data import GameCenterLeaderboardSetCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetCreateRequestData from a JSON string
game_center_leaderboard_set_create_request_data_instance = GameCenterLeaderboardSetCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_set_create_request_data_dict = game_center_leaderboard_set_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardSetCreateRequestData from a dict
game_center_leaderboard_set_create_request_data_from_dict = GameCenterLeaderboardSetCreateRequestData.from_dict(game_center_leaderboard_set_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


