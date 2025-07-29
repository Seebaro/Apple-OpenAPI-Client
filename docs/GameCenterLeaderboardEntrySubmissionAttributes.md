# GameCenterLeaderboardEntrySubmissionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bundle_id** | **str** |  | [optional] 
**challenge_ids** | **List[str]** |  | [optional] 
**context** | **decimal.Decimal** |  | [optional] 
**scoped_player_id** | **str** |  | [optional] 
**score** | **decimal.Decimal** |  | [optional] 
**submitted_date** | **datetime** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission_attributes import GameCenterLeaderboardEntrySubmissionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmissionAttributes from a JSON string
game_center_leaderboard_entry_submission_attributes_instance = GameCenterLeaderboardEntrySubmissionAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmissionAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_attributes_dict = game_center_leaderboard_entry_submission_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmissionAttributes from a dict
game_center_leaderboard_entry_submission_attributes_from_dict = GameCenterLeaderboardEntrySubmissionAttributes.from_dict(game_center_leaderboard_entry_submission_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


