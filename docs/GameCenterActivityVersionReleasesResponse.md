# GameCenterActivityVersionReleasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterActivityVersionRelease]**](GameCenterActivityVersionRelease.md) |  | 
**included** | [**List[GameCenterActivityVersion]**](GameCenterActivityVersion.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_version_releases_response import GameCenterActivityVersionReleasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionReleasesResponse from a JSON string
game_center_activity_version_releases_response_instance = GameCenterActivityVersionReleasesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionReleasesResponse.to_json())

# convert the object into a dict
game_center_activity_version_releases_response_dict = game_center_activity_version_releases_response_instance.to_dict()
# create an instance of GameCenterActivityVersionReleasesResponse from a dict
game_center_activity_version_releases_response_from_dict = GameCenterActivityVersionReleasesResponse.from_dict(game_center_activity_version_releases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


