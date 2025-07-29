# GameCenterLeaderboardImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterLeaderboardImageCreateRequestDataRelationships**](GameCenterLeaderboardImageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_image_create_request_data import GameCenterLeaderboardImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardImageCreateRequestData from a JSON string
game_center_leaderboard_image_create_request_data_instance = GameCenterLeaderboardImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardImageCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_image_create_request_data_dict = game_center_leaderboard_image_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardImageCreateRequestData from a dict
game_center_leaderboard_image_create_request_data_from_dict = GameCenterLeaderboardImageCreateRequestData.from_dict(game_center_leaderboard_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


