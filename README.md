# Community Documentserver

## Requirements

The community document server only supports running on x86-64 Linux servers.

When installing from git `make` and `docker` are required.

## Configuring OnlyOffice

The community documentserver will automatically configure itself if no other document server is configured in the onlyoffice settings ("Document Editing Service address" is empty).
All other "Server settings" should be left empty.

## Setup from git

- clone the repo into the Nextcloud app directory 
- run `make` in the app folder to download the 3rdparty components
- Enable the app

# OnlyOffice components

This app includes components from OnlyOffice to do a large part of the work.
While building the app, these components are copied over from the official OnlyOffice documentserver docker image (see `Makefile`).
The source for this can be found at the [OnlyOffice](https://github.com/ONLYOFFICE) github,
primarily the [web-apps](https://github.com/ONLYOFFICE/web-apps), [sdkjs](https://github.com/ONLYOFFICE/sdkjs) and [core](https://github.com/ONLYOFFICE/core) repositories.

These components are licenced under AGPL-3.0 with their copyright belonging to the OnlyOffice team.
