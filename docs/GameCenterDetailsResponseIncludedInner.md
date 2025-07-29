# GameCenterDetailsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionAttributes**](AppStoreVersionAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionRelationships**](AppStoreVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_details_response_included_inner import GameCenterDetailsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailsResponseIncludedInner from a JSON string
game_center_details_response_included_inner_instance = GameCenterDetailsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_details_response_included_inner_dict = game_center_details_response_included_inner_instance.to_dict()
# create an instance of GameCenterDetailsResponseIncludedInner from a dict
game_center_details_response_included_inner_from_dict = GameCenterDetailsResponseIncludedInner.from_dict(game_center_details_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


