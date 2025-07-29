# GameCenterDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterDetail**](GameCenterDetail.md) |  | 
**included** | [**List[GameCenterDetailsResponseIncludedInner]**](GameCenterDetailsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_detail_response import GameCenterDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailResponse from a JSON string
game_center_detail_response_instance = GameCenterDetailResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailResponse.to_json())

# convert the object into a dict
game_center_detail_response_dict = game_center_detail_response_instance.to_dict()
# create an instance of GameCenterDetailResponse from a dict
game_center_detail_response_from_dict = GameCenterDetailResponse.from_dict(game_center_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


