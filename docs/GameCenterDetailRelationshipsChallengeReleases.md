# GameCenterDetailRelationshipsChallengeReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterChallengeVersionRelationshipsReleasesDataInner]**](GameCenterChallengeVersionRelationshipsReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_challenge_releases import GameCenterDetailRelationshipsChallengeReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsChallengeReleases from a JSON string
game_center_detail_relationships_challenge_releases_instance = GameCenterDetailRelationshipsChallengeReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsChallengeReleases.to_json())

# convert the object into a dict
game_center_detail_relationships_challenge_releases_dict = game_center_detail_relationships_challenge_releases_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsChallengeReleases from a dict
game_center_detail_relationships_challenge_releases_from_dict = GameCenterDetailRelationshipsChallengeReleases.from_dict(game_center_detail_relationships_challenge_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


