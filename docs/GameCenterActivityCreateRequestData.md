# GameCenterActivityCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterActivityCreateRequestDataAttributes**](GameCenterActivityCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterAchievementCreateRequestDataRelationships**](GameCenterAchievementCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_create_request_data import GameCenterActivityCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityCreateRequestData from a JSON string
game_center_activity_create_request_data_instance = GameCenterActivityCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityCreateRequestData.to_json())

# convert the object into a dict
game_center_activity_create_request_data_dict = game_center_activity_create_request_data_instance.to_dict()
# create an instance of GameCenterActivityCreateRequestData from a dict
game_center_activity_create_request_data_from_dict = GameCenterActivityCreateRequestData.from_dict(game_center_activity_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


