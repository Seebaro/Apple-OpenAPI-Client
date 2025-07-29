# GameCenterChallengeVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**challenge** | [**GameCenterChallengeVersionRelationshipsChallenge**](GameCenterChallengeVersionRelationshipsChallenge.md) |  | [optional] 
**localizations** | [**GameCenterChallengeVersionRelationshipsLocalizations**](GameCenterChallengeVersionRelationshipsLocalizations.md) |  | [optional] 
**releases** | [**GameCenterChallengeVersionRelationshipsReleases**](GameCenterChallengeVersionRelationshipsReleases.md) |  | [optional] 
**default_image** | [**GameCenterChallengeLocalizationRelationshipsImage**](GameCenterChallengeLocalizationRelationshipsImage.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_version_relationships import GameCenterChallengeVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionRelationships from a JSON string
game_center_challenge_version_relationships_instance = GameCenterChallengeVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionRelationships.to_json())

# convert the object into a dict
game_center_challenge_version_relationships_dict = game_center_challenge_version_relationships_instance.to_dict()
# create an instance of GameCenterChallengeVersionRelationships from a dict
game_center_challenge_version_relationships_from_dict = GameCenterChallengeVersionRelationships.from_dict(game_center_challenge_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


