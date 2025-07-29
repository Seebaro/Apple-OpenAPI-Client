# GameCenterLeaderboardEntrySubmissionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes**](GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission_create_request_data import GameCenterLeaderboardEntrySubmissionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequestData from a JSON string
game_center_leaderboard_entry_submission_create_request_data_instance = GameCenterLeaderboardEntrySubmissionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmissionCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_create_request_data_dict = game_center_leaderboard_entry_submission_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequestData from a dict
game_center_leaderboard_entry_submission_create_request_data_from_dict = GameCenterLeaderboardEntrySubmissionCreateRequestData.from_dict(game_center_leaderboard_entry_submission_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


