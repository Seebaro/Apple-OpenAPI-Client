# GameCenterChallengeVersionRelationshipsReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterChallengeVersionRelationshipsReleasesDataInner]**](GameCenterChallengeVersionRelationshipsReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_version_relationships_releases import GameCenterChallengeVersionRelationshipsReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionRelationshipsReleases from a JSON string
game_center_challenge_version_relationships_releases_instance = GameCenterChallengeVersionRelationshipsReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionRelationshipsReleases.to_json())

# convert the object into a dict
game_center_challenge_version_relationships_releases_dict = game_center_challenge_version_relationships_releases_instance.to_dict()
# create an instance of GameCenterChallengeVersionRelationshipsReleases from a dict
game_center_challenge_version_relationships_releases_from_dict = GameCenterChallengeVersionRelationshipsReleases.from_dict(game_center_challenge_version_relationships_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


