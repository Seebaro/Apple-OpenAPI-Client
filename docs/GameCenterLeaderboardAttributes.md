# GameCenterLeaderboardAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**default_formatter** | [**GameCenterLeaderboardFormatter**](GameCenterLeaderboardFormatter.md) |  | [optional] 
**reference_name** | **str** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 
**submission_type** | **str** |  | [optional] 
**score_sort_type** | **str** |  | [optional] 
**score_range_start** | **decimal.Decimal** |  | [optional] 
**score_range_end** | **decimal.Decimal** |  | [optional] 
**recurrence_start_date** | **datetime** |  | [optional] 
**recurrence_duration** | **str** |  | [optional] 
**recurrence_rule** | **str** |  | [optional] 
**archived** | **bool** |  | [optional] 
**activity_properties** | **Dict[str, str]** |  | [optional] 
**visibility** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_attributes import GameCenterLeaderboardAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardAttributes from a JSON string
game_center_leaderboard_attributes_instance = GameCenterLeaderboardAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_attributes_dict = game_center_leaderboard_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardAttributes from a dict
game_center_leaderboard_attributes_from_dict = GameCenterLeaderboardAttributes.from_dict(game_center_leaderboard_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


