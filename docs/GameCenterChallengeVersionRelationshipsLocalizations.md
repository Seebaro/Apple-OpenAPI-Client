# GameCenterChallengeVersionRelationshipsLocalizations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterChallengeImageCreateRequestDataRelationshipsLocalizationData]**](GameCenterChallengeImageCreateRequestDataRelationshipsLocalizationData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_version_relationships_localizations import GameCenterChallengeVersionRelationshipsLocalizations

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionRelationshipsLocalizations from a JSON string
game_center_challenge_version_relationships_localizations_instance = GameCenterChallengeVersionRelationshipsLocalizations.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionRelationshipsLocalizations.to_json())

# convert the object into a dict
game_center_challenge_version_relationships_localizations_dict = game_center_challenge_version_relationships_localizations_instance.to_dict()
# create an instance of GameCenterChallengeVersionRelationshipsLocalizations from a dict
game_center_challenge_version_relationships_localizations_from_dict = GameCenterChallengeVersionRelationshipsLocalizations.from_dict(game_center_challenge_version_relationships_localizations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


