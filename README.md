# Fitbit Homeassistant

![languages](https://img.shields.io/badge/languages-JavaScript%20|%20CSS-blue)
![platform](https://img.shields.io/badge/platforms-Ionic%20|%20Versa%20|%20Versa%202%20|%20Versa%20Lite-silver)
![version](https://img.shields.io/badge/version-%200.2.0-green)
[![](https://img.shields.io/github/license/smirko-dev/fitbit-homeassistant.svg)](https://github.com/smirko-dev/fitbit-homeassistant/blob/master/LICENSE)
[![FitbitBuild Actions Status](https://github.com/smirko-dev/fitbit-homeassistant/workflows/FitbitBuild/badge.svg)](https://github.com/smirko-dev/fitbit-homeassistant/actions)
[![CodeQL Actions Status](https://github.com/smirko-dev/fitbit-homeassistant/workflows/CodeQL/badge.svg)](https://github.com/smirko-dev/fitbit-clohomeassistantckface/actions)

## Description

This app allows to control [Home Assistant](https://www.home-assistant.io/) entities from a [Fitbit watch](https://www.fitbit.com/global/eu/home).

Supported languages: de-DE, en-US.

Currently only entities are supported which can be turned on and off.

App icon is from https://icon-icons.com/de/symbol/home-assistant/138491 ([Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)).

### Requirements

Homeassistant accessible via https (this is a fitbit restriction).

A homeassistant token, described in [Authentication](https://www.home-assistant.io/docs/authentication/).

### Settings

Both, URL and Token can be setup in the app settings.

The settings also include a list to add entities by their ID (not name!).

## Screenshots

![App](screenshots/app.png)

## How to build

```
git clone git@github.com:smirko-dev/fitbit-homeassistant.git
cd fitbit-homeassistant
npm add --also=dev @fitbit/sdk
npm add --also=dev @fitbit/sdk-cli
npx fitbit-build generate-appid
npx fitbit-build
```
