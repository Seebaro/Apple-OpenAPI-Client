# GameCenterLeaderboardEntrySubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardEntrySubmissionAttributes**](GameCenterLeaderboardEntrySubmissionAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission import GameCenterLeaderboardEntrySubmission

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmission from a JSON string
game_center_leaderboard_entry_submission_instance = GameCenterLeaderboardEntrySubmission.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmission.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_dict = game_center_leaderboard_entry_submission_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmission from a dict
game_center_leaderboard_entry_submission_from_dict = GameCenterLeaderboardEntrySubmission.from_dict(game_center_leaderboard_entry_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


