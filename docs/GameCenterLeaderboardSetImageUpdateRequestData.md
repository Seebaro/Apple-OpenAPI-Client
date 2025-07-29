# GameCenterLeaderboardSetImageUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventScreenshotUpdateRequestDataAttributes**](AppEventScreenshotUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_image_update_request_data import GameCenterLeaderboardSetImageUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetImageUpdateRequestData from a JSON string
game_center_leaderboard_set_image_update_request_data_instance = GameCenterLeaderboardSetImageUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetImageUpdateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_set_image_update_request_data_dict = game_center_leaderboard_set_image_update_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardSetImageUpdateRequestData from a dict
game_center_leaderboard_set_image_update_request_data_from_dict = GameCenterLeaderboardSetImageUpdateRequestData.from_dict(game_center_leaderboard_set_image_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


