# {{ cookiecutter.application_name }}

{{ cookiecutter.description }}

## Build App For Release

```
make pack
```

This will package the app as `{{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}.zip`.

## Deploy

In the ThreatConnect UI install the App (the `.zip` file) created in the [Build App for Release](#build-app-for-release) section.

## Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and [Floyd Hightower's Spaces App Template](https://github.com/fhightower-templates/threatconnect-js-spaces-template).
