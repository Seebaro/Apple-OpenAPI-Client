# UserInvitationRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**visible_apps** | [**BetaTesterRelationshipsApps**](BetaTesterRelationshipsApps.md) |  | [optional] 

## Example

```python
from openapi_client.models.user_invitation_relationships import UserInvitationRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of UserInvitationRelationships from a JSON string
user_invitation_relationships_instance = UserInvitationRelationships.from_json(json)
# print the JSON string representation of the object
print(UserInvitationRelationships.to_json())

# convert the object into a dict
user_invitation_relationships_dict = user_invitation_relationships_instance.to_dict()
# create an instance of UserInvitationRelationships from a dict
user_invitation_relationships_from_dict = UserInvitationRelationships.from_dict(user_invitation_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


