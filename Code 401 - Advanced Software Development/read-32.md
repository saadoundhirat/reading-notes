# About Drf Permission

- Django REST framework is a powerful and flexible toolkit that makes it easy to build Web APIs. It provides class based generic API views and serializers. We've taken all the attributes and methods that every view/serializer defines or inherits, and flattened all that information onto one comprehensive page per class.
- Permissions in REST framework are always defined as a list of permission classes.

- Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.
- When the permissions checks fail either a "403 Forbidden" or a "401 Unauthorized" response will be returned, according to the following rules:
- The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers.
— An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.

## Object level permissions

REST framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.
Object level permissions are run by REST framework's generic views when .get_object() is called. As with view level permissions, an exceptions.PermissionDenied exception will be raised if the user is not allowed to act on the given object.
If you're writing your own views and want to enforce object level permissions, or if you override the get_object method on a generic view, then you'll need to explicitly call the .check_object_permissions(request, obj) method on the view at the point at which you've retrieved the object.
This will either raise a PermissionDenied or NotAuthenticated exception, or simply return if the view has the appropriate permissions.

- For example:

```
def get_object(self):
    obj = get_object_or_404(self.get_queryset (), pk=self.kwargs ["pk"])
    self.check_object_permissions(self.request, obj)
    return obj
```

## Generic views

- Django’s generic views... were developed as a shortcut for common usage patterns... They take certain common idioms and patterns found in view development and abstract them so that you can quickly write common views of data without having to repeat yourself.

Generic views
Django’s generic views... were developed as a shortcut for common usage patterns... They take certain common idioms and patterns found in view development and abstract them so that you can quickly write common views of data without having to repeat yourself.
