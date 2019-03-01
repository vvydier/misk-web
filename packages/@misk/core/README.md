## Misk Core

![](https://raw.githubusercontent.com/square/misk/master/misk.png)
This package provides shared, styled React components, Redux helper functions, and Typescript utilities across Misk tab repos. The top of each component/container file contains a usage example.

## Getting Started

```bash
$ yarn add @misk/core
```

## Builders

- `createApp(routes)`: builder function to create an `<App history={history}/>` component
- `createIndex(tabSlug, App, Ducks)`: builder function to create bootstrapping objects necessary for `index.tsx`

## Components

- `ErrorCalloutComponent`: Processes a Redux / Axios error and dumps raw JSON for debugging
- `OfflineComponent`: NonIdealState component for Offline or Loading tab state
- `PathDebugComponent`: outputs values passed in by props for `hash`, `pathname`, and `search` in React-Router instance
- `SidebarComponent`: dashboard styled sidebar

## Containers

- `DesktopWideOnlyContainer`: Only shows container when window width >1200px
- `FlexContainer`: Container using CSS FlexBox to have enclosed items flow responsively to screen width
- `MobileNeverContainer`: Never show container when window width <768px
- `MobileOnlyContainer`: Only show container when window width <768px
- `ResponsiveContainer`: Responsive container that all tabs and Nav Navbar use to ensure consistent view width

## Ducks

- `routerDucks`: router management Redux-Sagas parts (actions, dispatcher, handlers, sagas, reducers, state interface)
- `simpleFormDucks`: a standardized set of form and input handler Redux-Sagas parts (actions, dispatcher, handlers, sagas, reducers, state interface)
- `simpleNetworkDucks`: a standardized set of Axios based request Redux-Sagas parts (actions, dispatcher, handlers, sagas, reducers, state interface)

## Features

- `Navbar`: Related components to a dashboard styled Navbar

## Utilities

- `environment`: various utilities helpful in environment (color, default visibilities...)
- `network`: wrapped functions around Axios requests to allow simplified syntax that with `async await` returns an object of `{ data, error }`.

## [Releasing](https://github.com/square/misk-web/blob/master/RELEASING.md)

## [Changelog (and Breaking Changes)](https://github.com/square/misk-web/blob/master/CHANGELOG.md)