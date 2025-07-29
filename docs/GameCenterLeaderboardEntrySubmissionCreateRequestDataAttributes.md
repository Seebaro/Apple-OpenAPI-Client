# GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bundle_id** | **str** |  | 
**challenge_ids** | **List[str]** |  | [optional] 
**context** | **decimal.Decimal** |  | [optional] 
**scoped_player_id** | **str** |  | 
**score** | **decimal.Decimal** |  | 
**submitted_date** | **datetime** |  | [optional] 
**vendor_identifier** | **str** |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_entry_submission_create_request_data_attributes import GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes from a JSON string
game_center_leaderboard_entry_submission_create_request_data_attributes_instance = GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_entry_submission_create_request_data_attributes_dict = game_center_leaderboard_entry_submission_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes from a dict
game_center_leaderboard_entry_submission_create_request_data_attributes_from_dict = GameCenterLeaderboardEntrySubmissionCreateRequestDataAttributes.from_dict(game_center_leaderboard_entry_submission_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


