# GameCenterChallengeVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterChallengeImageCreateRequestDataRelationshipsVersionData]**](GameCenterChallengeImageCreateRequestDataRelationshipsVersionData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_versions_linkages_response import GameCenterChallengeVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionsLinkagesResponse from a JSON string
game_center_challenge_versions_linkages_response_instance = GameCenterChallengeVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionsLinkagesResponse.to_json())

# convert the object into a dict
game_center_challenge_versions_linkages_response_dict = game_center_challenge_versions_linkages_response_instance.to_dict()
# create an instance of GameCenterChallengeVersionsLinkagesResponse from a dict
game_center_challenge_versions_linkages_response_from_dict = GameCenterChallengeVersionsLinkagesResponse.from_dict(game_center_challenge_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


