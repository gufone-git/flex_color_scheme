[![Pub Version](https://img.shields.io/pub/v/flex_color_scheme?label=flex_color_scheme&labelColor=333940&logo=dart)](https://pub.dev/packages/flex_color_scheme) ![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/rydmike/flex_color_scheme/Test?event=push)
![Test](https://github.com/rydmike/flex_color_scheme/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/rydmike/flex_color_scheme/branch/master/graph/badge.svg?token=4XJU30IGO3)](https://codecov.io/gh/rydmike/flex_color_scheme) [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

# FlexColorScheme

[<img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/flutter-favorite-logo.png?raw=true?" alt="flutter favorite logo" width="170"/>](https://docs.flutter.dev/development/packages-and-plugins/favorites)

Use **FlexColorScheme** to make beautiful color scheme based Flutter themes,
with optional primary color surface blends, or key color seeded schemes.
The themes are based on the same concept as Flutter's ColorScheme based themes,
with many additional features and a large number of pre-made themes.

<table>
  <tr>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-l-37.png?raw=true" alt="Dash light" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-d-37.png?raw=true" alt="Dash dark" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-l-38.png?raw=true" alt="M3 baseline light" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-d-38.png?raw=true" alt="M3 baseline dark" width="220"/></td>
  </tr>
</table>

When you theme a Flutter application, all built-in widgets use the colors of the
`ColorScheme` in your theme. At least in theory, and it is almost so if you defined
your `ThemeData` by using the `ThemeData.from` factory, but it still misses
a few details.

**FlexColorScheme** ensures that all Flutter SDK widgets gets themed completely by its
color schemes and custom colors you provide. It also applies all the `ColorScheme` based colors
to all direct color properties in `ThemeData`, as long as they still exist. This
ensures that all the direct colors properties in `ThemeData` match your `ColorScheme`.

You can also opt-in on using opinionated component sub-themes.
By opting in, you can for example adjust the border radius on all UI widgets
with a single property value. Flutter's Material UI widgets still default to
being based on the Material 2 design, and thus use 4 dp corner radius on most
widgets.

When you opt-in on using the component sub-themes, the border radius on widgets
default to the new rounded corners as specified by the
[Material 3 guide](https://m3.material.io/), where the
radius varies by widget type. You can keep this, or set the global widget
radius to a value you prefer. You can also easily set the themed border
radius per widget, and override the Material 3 default or the global radius
value you defined.

<table>
  <tr>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-l-39.png?raw=true" alt="Verdun green light" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-d-39.png?raw=true" alt="Verdun green dark" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-l-40.png?raw=true" alt="Dell genoa light" width="220"/></td>
    <td><img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-d-40.png?raw=true" alt="Dell genoa dark" width="220"/></td>
  </tr>
</table>

With **FlexColorScheme** sub-themes you use simple flat component property values.
No need for verbose Flutter SDK component sub-themes, with `ShapeBorder`
definitions on multiple widget themes to change their border radius. The component
sub-theming provides a large amount of easy to configure options via simple flat
properties, instead of complicated nested ones. In many cases you can also completely
avoid the both complicated and confusing `MaterialState` callback theming properties.

**FlexColorScheme** also has many advanced coloring features, like using
surface alpha blends. It also fully supports Material 3 based color schemes,
including seed key color generated `ColorSchemes`. It offers many configuration
options that you can use when you generate your `ColorScheme` from
key colors, features that are currently not available in Flutter.

## Documentation

FlexColorSchemes has a dedicated documentation site
[**docs.flexcolorscheme.com**](https://docs.flexcolorscheme.com/).
Please refer to it for more information and tutorials on its usage and features.
The documentation site is powered by [docs.page](https://docs.page/)
from [Invertase](https://invertase.io/).

Complete generated package
[API documentation](https://pub.dev/documentation/flex_color_scheme/latest/flex_color_scheme/flex_color_scheme-library.html)
is also available.

## Themes Playground

If you are here for the **FlexColorScheme** companion application that allows you
to configure a FlexColorScheme theme, and copy-paste its setup code for use in
your application, then launch the
[**Themes Playground app here**](https://rydmike.com/flexcolorscheme/themesplayground-v5).

[<img src="https://github.com/rydmike/flex_color_scheme_docs/blob/master/docs/images/fcs-v5-pg-01-pageview-3.gif?raw=true" alt="Page view demo"/>](https://rydmike.com/flexcolorscheme/themesplayground-v5)
