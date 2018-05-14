# Cura Plugin OAuth2 Module
A python module for out-of-the-box OAuth2 client support for Cura plugins.

## Installation
The safest way of installing this module is using git submodule.
This is handy because Cura plugins require all the dependencies to be in the packaged plugin.

```
git submodule add git@github.com:Ultimaker/CuraPluginOAuth2Module.git lib/CuraPluginOAuth2Module
```

## Usage
Simply include the `AuthorizationService` like you would with any other Python class.
The samples here assume you have loaded the module as git submodule under `/lib/CuraPluginOAuth2Module`.
Make sure there is an `__init__.py` in your `/lib` folder as well!

```python
from lib.CuraPluginOAuth2Module.OAuth2Client.AuthorizationService import AuthorizationService
from lib.CuraPluginOAuth2Module.OAuth2Client.models import OAuth2Settings

auth_settings = OAuth2Settings(
    # Place actual auth settings here.
)
auth_service = AuthorizationService(auth_settings)
```

More documentation will follow soon.

## Maintenance
The current active maintainer of this repository is <c.terbeke@ultimaker.com>. Please contact me for questions.

## License
CuraPluginOAuth2Module is released under the terms of the LGPLv3 or higher.
A copy of this license should be included with the software.
