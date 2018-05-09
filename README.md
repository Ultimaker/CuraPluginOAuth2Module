# Cura Plugin OAuth2 Module
A python module for out-of-the-box OAuth2 client support for Cura plugins.

## Installation
You can either use `pip install` or `git submodule` to install the module.

```bash
pip install https://github.com/Ultimaker/CuraPluginOAuth2Module
```

```
git submodule add https://github.com/Ultimaker/CuraPluginOAuth2Module lib/CuraPluginOAuth2Module
```

## Usage
Simply include the `AuthorizationService` like you would with any other Python class.
The samples here assume you have loaded the module as git submodule.

```python
from lib.CuraPluginOAuth2Module.OAuth2Client.AuthorizationService import AuthorizationService
from lib.CuraPluginOAuth2Module.OAuth2Client.models import OAuth2Settings

auth_settings = OAuth2Settings(

)
auth_service = AuthorizationService(auth_settings)
```

## Maintenance
The current active maintainer of this repository is <c.terbeke@ultimaker.com>. Please contact me for questions.
