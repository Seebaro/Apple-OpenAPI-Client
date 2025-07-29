# GameCenterActivityResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivity**](GameCenterActivity.md) |  | 
**included** | [**List[GameCenterActivitiesResponseIncludedInner]**](GameCenterActivitiesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_response import GameCenterActivityResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityResponse from a JSON string
game_center_activity_response_instance = GameCenterActivityResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityResponse.to_json())

# convert the object into a dict
game_center_activity_response_dict = game_center_activity_response_instance.to_dict()
# create an instance of GameCenterActivityResponse from a dict
game_center_activity_response_from_dict = GameCenterActivityResponse.from_dict(game_center_activity_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


