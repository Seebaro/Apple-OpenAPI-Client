# GameCenterActivityVersionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterActivityVersionCreateRequestDataAttributes**](GameCenterActivityVersionCreateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**GameCenterActivityVersionCreateRequestDataRelationships**](GameCenterActivityVersionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_create_request_data import GameCenterActivityVersionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionCreateRequestData from a JSON string
game_center_activity_version_create_request_data_instance = GameCenterActivityVersionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionCreateRequestData.to_json())

# convert the object into a dict
game_center_activity_version_create_request_data_dict = game_center_activity_version_create_request_data_instance.to_dict()
# create an instance of GameCenterActivityVersionCreateRequestData from a dict
game_center_activity_version_create_request_data_from_dict = GameCenterActivityVersionCreateRequestData.from_dict(game_center_activity_version_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


