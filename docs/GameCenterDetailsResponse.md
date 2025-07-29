# GameCenterDetailsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterDetail]**](GameCenterDetail.md) |  | 
**included** | [**List[GameCenterDetailsResponseIncludedInner]**](GameCenterDetailsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_details_response import GameCenterDetailsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailsResponse from a JSON string
game_center_details_response_instance = GameCenterDetailsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailsResponse.to_json())

# convert the object into a dict
game_center_details_response_dict = game_center_details_response_instance.to_dict()
# create an instance of GameCenterDetailsResponse from a dict
game_center_details_response_from_dict = GameCenterDetailsResponse.from_dict(game_center_details_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


