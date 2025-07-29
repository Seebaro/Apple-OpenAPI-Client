# GameCenterLeaderboardCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterLeaderboardCreateRequestDataAttributes**](GameCenterLeaderboardCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterLeaderboardCreateRequestDataRelationships**](GameCenterLeaderboardCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_create_request_data import GameCenterLeaderboardCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardCreateRequestData from a JSON string
game_center_leaderboard_create_request_data_instance = GameCenterLeaderboardCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_create_request_data_dict = game_center_leaderboard_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardCreateRequestData from a dict
game_center_leaderboard_create_request_data_from_dict = GameCenterLeaderboardCreateRequestData.from_dict(game_center_leaderboard_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


