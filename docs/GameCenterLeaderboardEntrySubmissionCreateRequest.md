# GameCenterLeaderboardEntrySubmissionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardEntrySubmissionCreateRequestData**](GameCenterLeaderboardEntrySubmissionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission_create_request import GameCenterLeaderboardEntrySubmissionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequest from a JSON string
game_center_leaderboard_entry_submission_create_request_instance = GameCenterLeaderboardEntrySubmissionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmissionCreateRequest.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_create_request_dict = game_center_leaderboard_entry_submission_create_request_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequest from a dict
game_center_leaderboard_entry_submission_create_request_from_dict = GameCenterLeaderboardEntrySubmissionCreateRequest.from_dict(game_center_leaderboard_entry_submission_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


