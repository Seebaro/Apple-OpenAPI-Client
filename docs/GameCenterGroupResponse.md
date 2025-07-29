# GameCenterGroupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterGroup**](GameCenterGroup.md) |  | 
**included** | [**List[GameCenterGroupsResponseIncludedInner]**](GameCenterGroupsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_group_response import GameCenterGroupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroupResponse from a JSON string
game_center_group_response_instance = GameCenterGroupResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroupResponse.to_json())

# convert the object into a dict
game_center_group_response_dict = game_center_group_response_instance.to_dict()
# create an instance of GameCenterGroupResponse from a dict
game_center_group_response_from_dict = GameCenterGroupResponse.from_dict(game_center_group_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


