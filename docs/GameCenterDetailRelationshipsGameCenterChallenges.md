# GameCenterDetailRelationshipsGameCenterChallenges


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterChallengeVersionRelationshipsChallengeData]**](GameCenterChallengeVersionRelationshipsChallengeData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_game_center_challenges import GameCenterDetailRelationshipsGameCenterChallenges

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsGameCenterChallenges from a JSON string
game_center_detail_relationships_game_center_challenges_instance = GameCenterDetailRelationshipsGameCenterChallenges.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsGameCenterChallenges.to_json())

# convert the object into a dict
game_center_detail_relationships_game_center_challenges_dict = game_center_detail_relationships_game_center_challenges_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsGameCenterChallenges from a dict
game_center_detail_relationships_game_center_challenges_from_dict = GameCenterDetailRelationshipsGameCenterChallenges.from_dict(game_center_detail_relationships_game_center_challenges_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


