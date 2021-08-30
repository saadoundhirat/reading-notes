# Django CRUD and Forms

- An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

    ![](https://3.bp.blogspot.com/-Z1r1rv1HpNU/XpQg2WlAW5I/AAAAAAAAWtg/Fa8kMATByIUsGhwpgYy_f3HThQ5CqP_yQCLcBGAsYHQ/s1600/django_crud.jpg)


## Django form handling process

- Display the default form the first time it is requested by the user.
The form may contain blank fields (e.g. if you're creating a new record), or it may be pre-populated with initial values (e.g. if you are changing a record, or have useful default initial values).
- The form is referred to as unbound at this point, because it isn't associated with any user-entered data (though it may have initial values).
Receive data from a submit request and bind it to the form.
- Binding data to the form means that the user-entered data and any errors are available when we need to redisplay the form.
Clean and validate the data.
- Cleaning the data performs sanitization of the input (e.g. removing invalid characters that might be used to send malicious content to the server) and converts them into consistent Python types.
- Validation checks that the values are appropriate for the field (e.g. are in the right date range, aren't too short or too long, etc.)
If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.
If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)
- Once all actions are complete, redirect the user to another page.

## ModelForms

- Creating a Form class using the approach described above is very flexible, allowing you to create whatever sort of form page you like and associate it with any model or models.

- However, if you just need a form to map the fields of a single model then your model will already define most of the information that you need in your form: fields, labels, help text and so on. Rather than recreating the model definitions in your form, it is easier to use the ModelForm helper class to create the form from your model. This ModelForm can then be used within your views in exactly the same way as an ordinary Form.

A basic ModelForm containing the same field as our original RenewBookForm is shown below. All you need to do to create the form is add class Meta with the associated model (BookInstance) and a list of the model fields to include in the form.

```
from django.forms import ModelForm
from catalog.models import BookInstance

class RenewBookModelForm(ModelForm):
    class Meta:
        model = BookInstance
        fields = ['due_back']
```


## Templates

The "create" and "update" views use the same template by default, which will be named after your model: model_name_form.html (you can change the suffix to something other than _form using the template_name_suffix field in your view, for example template_name_suffix = '_other_suffix')
