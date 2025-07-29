# GameCenterGroupsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterGroup]**](GameCenterGroup.md) |  | 
**included** | [**List[GameCenterGroupsResponseIncludedInner]**](GameCenterGroupsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_groups_response import GameCenterGroupsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroupsResponse from a JSON string
game_center_groups_response_instance = GameCenterGroupsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroupsResponse.to_json())

# convert the object into a dict
game_center_groups_response_dict = game_center_groups_response_instance.to_dict()
# create an instance of GameCenterGroupsResponse from a dict
game_center_groups_response_from_dict = GameCenterGroupsResponse.from_dict(game_center_groups_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


