# GameCenterActivityVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity** | [**GameCenterActivityVersionRelationshipsActivity**](GameCenterActivityVersionRelationshipsActivity.md) |  | [optional] 
**localizations** | [**GameCenterActivityVersionRelationshipsLocalizations**](GameCenterActivityVersionRelationshipsLocalizations.md) |  | [optional] 
**default_image** | [**GameCenterActivityLocalizationRelationshipsImage**](GameCenterActivityLocalizationRelationshipsImage.md) |  | [optional] 
**releases** | [**GameCenterActivityVersionRelationshipsReleases**](GameCenterActivityVersionRelationshipsReleases.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_version_relationships import GameCenterActivityVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionRelationships from a JSON string
game_center_activity_version_relationships_instance = GameCenterActivityVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionRelationships.to_json())

# convert the object into a dict
game_center_activity_version_relationships_dict = game_center_activity_version_relationships_instance.to_dict()
# create an instance of GameCenterActivityVersionRelationships from a dict
game_center_activity_version_relationships_from_dict = GameCenterActivityVersionRelationships.from_dict(game_center_activity_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


