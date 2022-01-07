# Modified [telegram](https://www.home-assistant.io/integrations/telegram/) component for Home Assistant

## Installation
*__Manual mode__*

Place the `telegram_mod` folder into your `custom_components` folder.

*__Adding custom repository to [HACS](https://hacs.xyz/)__*

Go to the Integrations page in HACS and select the three dots in the top right corner. Select Custom repositories.
Add repository url. Category - Integration. Read more on https://hacs.xyz/docs/faq/custom_repositories.

## Changes compared to the original component

* Added `message_tag`.
* Added `disable_notification`
* Added `parse_mode`

## Example
```yaml
# Example configuration.yaml entry
- service: notify.telegram
  data:
    message: "message"
    title: "title"
    data:
      message_tag: "message_tag"
      disable_notification: True
      parse_mode: html
```
