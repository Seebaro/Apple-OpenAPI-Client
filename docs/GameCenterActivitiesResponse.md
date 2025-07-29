# GameCenterActivitiesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterActivity]**](GameCenterActivity.md) |  | 
**included** | [**List[GameCenterActivitiesResponseIncludedInner]**](GameCenterActivitiesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activities_response import GameCenterActivitiesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivitiesResponse from a JSON string
game_center_activities_response_instance = GameCenterActivitiesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivitiesResponse.to_json())

# convert the object into a dict
game_center_activities_response_dict = game_center_activities_response_instance.to_dict()
# create an instance of GameCenterActivitiesResponse from a dict
game_center_activities_response_from_dict = GameCenterActivitiesResponse.from_dict(game_center_activities_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


