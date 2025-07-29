# GameCenterActivityVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterActivityVersion]**](GameCenterActivityVersion.md) |  | 
**included** | [**List[GameCenterActivityVersionsResponseIncludedInner]**](GameCenterActivityVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_versions_response import GameCenterActivityVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionsResponse from a JSON string
game_center_activity_versions_response_instance = GameCenterActivityVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionsResponse.to_json())

# convert the object into a dict
game_center_activity_versions_response_dict = game_center_activity_versions_response_instance.to_dict()
# create an instance of GameCenterActivityVersionsResponse from a dict
game_center_activity_versions_response_from_dict = GameCenterActivityVersionsResponse.from_dict(game_center_activity_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


