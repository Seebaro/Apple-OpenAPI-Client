# GameCenterLeaderboardEntrySubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardEntrySubmission**](GameCenterLeaderboardEntrySubmission.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission_response import GameCenterLeaderboardEntrySubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmissionResponse from a JSON string
game_center_leaderboard_entry_submission_response_instance = GameCenterLeaderboardEntrySubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmissionResponse.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_response_dict = game_center_leaderboard_entry_submission_response_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmissionResponse from a dict
game_center_leaderboard_entry_submission_response_from_dict = GameCenterLeaderboardEntrySubmissionResponse.from_dict(game_center_leaderboard_entry_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


