# GameCenterChallengeRelationshipsVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterChallengeImageCreateRequestDataRelationshipsVersionData]**](GameCenterChallengeImageCreateRequestDataRelationshipsVersionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_relationships_versions import GameCenterChallengeRelationshipsVersions

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeRelationshipsVersions from a JSON string
game_center_challenge_relationships_versions_instance = GameCenterChallengeRelationshipsVersions.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeRelationshipsVersions.to_json())

# convert the object into a dict
game_center_challenge_relationships_versions_dict = game_center_challenge_relationships_versions_instance.to_dict()
# create an instance of GameCenterChallengeRelationshipsVersions from a dict
game_center_challenge_relationships_versions_from_dict = GameCenterChallengeRelationshipsVersions.from_dict(game_center_challenge_relationships_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


