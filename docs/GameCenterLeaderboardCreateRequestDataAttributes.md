# GameCenterLeaderboardCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**default_formatter** | [**GameCenterLeaderboardFormatter**](GameCenterLeaderboardFormatter.md) |  | 
**reference_name** | **str** |  | 
**vendor_identifier** | **str** |  | 
**submission_type** | **str** |  | 
**score_sort_type** | **str** |  | 
**score_range_start** | **decimal.Decimal** |  | [optional] 
**score_range_end** | **decimal.Decimal** |  | [optional] 
**recurrence_start_date** | **datetime** |  | [optional] 
**recurrence_duration** | **str** |  | [optional] 
**recurrence_rule** | **str** |  | [optional] 
**activity_properties** | **Dict[str, str]** |  | [optional] 
**visibility** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_create_request_data_attributes import GameCenterLeaderboardCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardCreateRequestDataAttributes from a JSON string
game_center_leaderboard_create_request_data_attributes_instance = GameCenterLeaderboardCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_create_request_data_attributes_dict = game_center_leaderboard_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardCreateRequestDataAttributes from a dict
game_center_leaderboard_create_request_data_attributes_from_dict = GameCenterLeaderboardCreateRequestDataAttributes.from_dict(game_center_leaderboard_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


