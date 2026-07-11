# User-Configuration
User Configuration Manager

A simple Python project for managing user settings stored in a dictionary. It supports adding, updating, deleting, and viewing configuration settings, with built-in validation and formatted output messages.

Features


Add a setting — Add a new key-value pair to the settings dictionary (fails gracefully if the key already exists).
Update a setting — Update the value of an existing setting (fails gracefully if the key doesn't exist).
Delete a setting — Remove a setting by key.
View settings — Display all current settings in a readable, formatted list.


All keys and values are automatically converted to lowercase for consistency, except when displaying settings, where key names are capitalized for readability.

Project Structure

user-configuration-manager/
settings.py/
README.md

Functions

add_setting(settings, key_value)

Adds a new setting to the settings dictionary.


settings: dict of existing settings
key_value: tuple of (key, value)


Returns a success message if added, or an error message if the key already exists.

update_setting(settings, key_value)

Updates an existing setting's value.


settings: dict of existing settings
key_value: tuple of (key, value)


Returns a success message if updated, or an error message if the key doesn't exist.

delete_setting(settings, key)

Deletes a setting by key.


settings: dict of existing settings
key: the setting name to remove


Returns a success message if deleted, or "Setting not found!" if the key doesn't exist.

view_settings(settings)

Returns a formatted string of all current settings, or "No settings available." if empty.
