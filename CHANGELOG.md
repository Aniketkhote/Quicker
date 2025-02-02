## 6.1.1

- Fixed color style according to material 3

## 6.1.0

### Added

- **Accessibility Enhancements**: Added `Semantics` support for better screen reader compatibility in `FxCheckbox`, `FxRadio`, `FxSwitch`, and `FxTextFormField`.
- **Customization Options**:
  - `isDisabled` property in `FxCheckbox` and `FxRadio` for disabling interactions with visual feedback.
  - `thumbColor` in `FxSwitch` and `innerCircleColor`, `innerCircleScale` in `FxRadio` for improved customization.
  - Optional `borderColor` for better visual customization in `FxSwitch`.
  - Customizable `animationDuration` in `FxShimmer` for flexible shimmer effects.
- **Dynamic Theming**: Support for dynamic theming in `FxCheckbox`, `FxRadio`, `FxSwitch`, and `FxTextFormField` to respect app’s theme colors.

### Changed

- **UI Updates**:
  - Replaced `GestureDetector` with `InkWell` in `FxCheckbox`, `FxRadio`, and `FxSwitch` for ripple effects and hover support.
  - Replaced `AnimatedBuilder` with `AnimatedContainer` in `FxShimmer` for better performance and simpler code.
  - Updated `FxTextFormField` to align with Material 3 guidelines, introducing `FilledTextField` and `OutlinedTextField` styles.
  - Renamed `onChange` to `onChanged` for consistency with Flutter conventions.
- **Input Decoration**:
  - Replaced custom border handling in `FxTextFormField` with `OutlineInputBorder` for consistent Material 3 border styles.
  - Added `filled` and `fillColor` properties in `FxTextFormField`.

### Improved

- **Performance**: Optimized code readability and modularity for better maintainability and smoother animations in `FxCheckbox`, `FxRadio`, `FxSwitch`, and `FxTextFormField`.
- **Shimmer Animation**: Refined shimmer effect with smoother transitions and customizable animation duration.
- **Focus and Error States**: Enhanced error and focus state handling in `FxTextFormField` for better user experience.

### Fixed

- **Color Handling**: Fixed color handling for active, inactive, and thumb states in `FxSwitch` and `FxRadio` to fallback to theme defaults when not specified.

## 6.0.0

### Added

- `child` widget in `FxButton` for more flexible content.
- Smooth animations in `FxCheckbox`, `FxRadio`, and `FxSwitch` for improved user experience.
- `inActive` field in `FxRadio` for better control over radio button states.
- `thumbColor` property in `FxSwitch` for customizable switch appearance.
- Additional fields in `FxTextFormField` for enhanced functionality.
- More granular offset options (`xsOffset`, `smOffset`, `mdOffset`, `lgOffset`, `xlOffset`) in place of a single `offset` for improved responsive design.

### Changed

- Renamed `onChange` function to `onChanged` in `FxCheckbox` for consistency with Flutter conventions.
- Renamed `isChecked` property to `value` in `FxCheckbox` for clarity.
- Renamed `Shimmer` widget to `FxShimmer` for consistency with library naming conventions.

### Improved

- Enhanced `FxGrid` and `FxResponsive` widgets for better performance and flexibility in responsive layouts.

## 5.8.0

### Added basic string manipulation methods

- `isPhone`: Validates if the string is a phone number.
- `isHexColor`: Validates if the string is a valid hexadecimal color code.
- `isCreditCard`: Validates if the string is a valid credit card number.
- `isJson`: Validates if the string is a valid JSON format.
- `isUUID`: Validates if the string is a valid UUID.
- `isHtml`: Checks if the string contains HTML.
- `isDate`: Validates if the string is a valid date in 'YYYY-MM-DD' format.
- `isTime`: Validates if the string is a valid time in 'HH' format.
- `isIPv4`: Validates if the string is a valid IPv4 address.
- `isIPv6`: Validates if the string is a valid IPv6 address.

### Transformation Methods

- `reverse`: Reverses the entire string.
- `removeDigits`: Removes all digits from the string.
- `removeSpecialChars`: Removes all special characters, leaving only alphanumeric values.
- `toggleCase`: Toggles the case of each character in the string (uppercase to lowercase and vice versa).

### Content Extraction

- `extractEmails`: Extracts all valid email addresses from the string.
- `extractUrls`: Extracts all valid URLs from the string.
- `removeHtmlTags`: Removes all HTML tags from the string.

## 5.7.0

- Added more validations.
- Fixed outline color isses in `FxButon`.

## 5.6.3

- Fixed border size isses in `FxButon`.
- Fixed padding isses in `FxTextFormField`.

## 5.6.2

- Fixed icon size isses in `FxButon`.

## 5.6.1

- Fixed padding issue in `FxButton`.
- Made text field optional in `FxButton`.

## 5.6.0

- Added only icon option for FxButton, which is now displayed centered.
- Replaced prefixIconSize and suffixIconSize with iconSize.

## 5.5.3

- Fixed linting issues.

## 5.5.2

- Fixed datatypes in list and map extension.

## 5.5.1

- Fixed helper function export issue.

## 5.5.0

- Added `generateOTP` and `generateAvatar` helper method.

## 5.4.0

- Added `isBool` and `isUrl` methods to String extensions.
- Added `devicePixelRatio` and `textScaleFactor` methods in Context extensions.
- Added `BorderColor` and `BoxShadow` methods in TextFormField.
- Enhanced the isEmail regex for improved accuracy.

## 5.3.0

- Added `delay` method in `Duration` and `num` extensions.

## 5.2.1

- Updated test cases to accommodate the new defaultValue parameter, ensuring comprehensive coverage and accurate functionality testing.

## 5.2.0

- Added support for the `defaultValue` parameter in the `getId`, `getString`, `getInt`, and `getDouble` methods.

## 5.1.0

- Added `removeNullValues()` method to Map extensions, which removes entries with null values from the map.
- Introduced shorthand getters such as `top5`, `top10`, `left5`, etc., allowing users to specify border radius for individual sides with specific values more conveniently.
- Added `Shimmer` widget for displaying a shimmer effect.

## 5.0.0

**Breaking changes**

- Removed Queue and Navigation. Instead of using Queue and Navigation, please use Refreshed package available at https://pub.dev/packages/refreshed.
- Renamed `diffForHumans` method to `timeAgo`.
- Changed boolean parameters in extension methods from positional parameters to named parameters.
- Added some more `DateTime` extensions.

## 4.2.7

- Fixed minor issues in list.

## 4.2.6

- Fixed pub points.

## 4.2.5

- Support for new SDK version `>=3.3.0 <4.0.0`.

## 4.2.4

- Support for new SDK version `>=3.2.6 <4.0.0`.

## 4.2.3

- The `FxButton` widget now has splash color set to false by default.

## 4.2.2

- Replaced the deprecated `TextScalarFactor` with `TextScalar`.
- Resolved the `FxButton` outline color issue.

## 4.2.1

- Minor improvements

## 4.2.0

**Added:**

- Added new widgets `FxCheckbox` , `FxRadio` and `FxSwitch`.
- Added extra parameter `textStyle` in FxButton.

**Fixed:**

- Fixed padding horizontal and vertical spacing issue in Padding Extension.
- Fixed Extra spacing in FxTextField icons.
- Fixed Icon Color issue in FxButon icons.

## 4.1.1

**Fixed:**

- Fixed extra spacing in FxTextField.

## 4.1.0

**Added:**

- Added prefix and suffix icon size params in FxButton.
- Added prefix and suffix icons params in FxTextFormField.

**Fixed:**

- Changed leadingIcon to prefixIcon and trailingIcon suffixIcon in FxButton.

## 4.0.3

**Fixed:**

- Improved Widget style.

## 4.0.2

**Fixed:**

- Improved FxNavigation.

## 4.0.1

**Fixed:**

- Revised and improved context extension methods.

## 4.0.0

**Breaking Changes:**

- Revised and improved the navigation, providing a better user experience and enhanced functionality.
- Revised and improved the Queue feature, making it more efficient and reliable.
- Improved the FxResponsive Widget, enhancing its responsiveness and adaptability.
- Modified the `hide` method to `hide()` to accept a condition, allowing for more flexible hiding options.
- Removed the `hideIf()` and `showIf()` extension methods from the Widget, streamlining the API and removing deprecated functionality.

**Added:**

- Introduced the `FxGrid` widget, which enables developers to create dynamic and responsive grid layouts.
- Implemented the `shadow` mixin, offering a simple and reusable way to apply shadows to widgets.
- Introduced the `FxButton` widget, providing a customizable button component with various styles and configurations.
- Added the `FxTextFormField` Widget, a text input field with built-in validation and error handling capabilities.
- Included the `Pick()` method in the map extension, allowing for easy retrieval of specific values from a map.
- Added the `diffForHumans` method to the map extension, enabling developers to obtain human-readable time differences.
- Expanded the `shimmer()` extension to support custom gradients, animations, and directions.
- Introduced transparent color support in the FxColor class.
- Added the text theme style extension on the build context, simplifying the application of consistent text styles.

**Fixed:**

- Resolved an issue causing an empty list exception in the `chunk()` function.
- Fixed a bug causing an empty list exception in the `split()` function.

## 3.6.4

- Corrected a typo in the README file.
- Expanded the functionality of the BuildContext class by adding some new extensions.
- Revised and improved the text cases for the Map extension.

## 3.6.3

- Resolved issues related to String extensions.
- Refactored test cases for extensions of String, Int, and Num types.

## 3.6.2

- Minor issues fixed.

## 3.6.1

- Improved type safety and null safety checks to reduce runtime errors.

## 3.6.0

- Added a Job and Queue feature to support asynchronous operations. The Queue class executes jobs one by one and has an add() method to add a job to the queue. The Job class represents a single unit of work and has an execute() method that completes the job's Completer with either the result of the function or an error if an exception is thrown.

- Added an extension to the FxNavigation class that supports custom route animations for navigating to pages using the `toPage()` and `toNamed()` methods. These methods also support passing arguments to the destination page.

- Added the `offPage()` and `offNamed()` methods to the FxNavigation class to replace the current page with a new one, with custom route animations.

- Added the `navigateTo()` method to the FxNavigation class to navigate to a new page with custom route animations, with an option to replace the current page.

- Added the `back()`, `canPop()`, and `maybePop()` methods to the FxNavigation class to handle navigation history. The `back()` method navigates to the previous page in the history stack. The `canPop()` method returns whether there is a page to go back to. The `maybePop()` method checks if there is a page to go back to and goes back if there is one.

## 3.5.0

- Fixed `Text Color` extension getters.
- Refined getters naming for the Fixed Text Color extension, such as changing `kcWarningLightStatus` to `kcWarningLight`.
- Deleted unneeded Text Color extension getters, including `kcText`, `kcLabel`, `kcDisabled`, and `kcTextField`.
- Improved the Extension code documentation to increase clarity and readability.
- Changed the application of the `BorderRadius` extension from the Container widget to the `ClipRRect` widget, allowing for improved control over rounded corners.
- Added the `Shimmer extension` to the Widget.

## 3.4.0

- Updated package dependencies to the latest versions of `Flutter (3.7.0)` and `Dart (2.19.0)`
- Expanded documentation to provide more detailed information
- Revised the **README.md** file to include additional examples and explanations.

## 3.3.0

- Implemented a new method `retainKeys()` in the Map extension to remove key-value pairs whose keys are not present in a given list.
- Removed methods related to text styling such as letter spacing, word spacing, line height and text decoration.
- Implemented checks to verify that the list is not empty and contains Map elements in the where methods to avoid runtime errors.
- Added type checking for the generic type T in the list extensions to ensure that the methods are only applied to lists of the correct type.
- Updated the documentation for the extension with proper examples and explanations for each method.

## 3.2.0

- Made improvements to the code for better performance and removed any unnecessary checks.
- Removed a dependency on the `get` package.

## 3.1.0

- Small corrections have been made to the package to address any minor issues.

## 3.0.0

- An update has been made to the stable version of flutter, bringing it to `version 3.3.8`. This update includes various improvements and bug fixes.

## 2.5.0

- Small corrections have been made to the package to address any minor issues.

## 2.4.0

### Fixed

- The default value for the functions `getInt` and `getDouble` have been corrected.
- Additionally, other bugs have been resolved.

## 2.3.0

### Added

- The widget extension now includes the option for `flexible`, allowing for more flexibility in layout and design.
- The radius radius extension has been added, allowing for more customization of the border corners.
- The list extension has been enhanced with new options for filtering and querying data, including `whereOnly`, `whereNotOnly`, `whereBetween`, `whereNotBetween`, `whereIn` and `whereNotIn`, providing more advanced options for data manipulation.

## 2.2.0

### Added

- Added some extra constant in padding extension
- Added `doesntContain()` method in map extension

### Changed

- Renamed main color names, such as "primary" to "kcPrimary" in Text extension.
- Slightly altered main color codes.
- Converted utility classes to mixins.

## 2.1.0

### Added

- The `groupBy()` function allows for grouping of list items based on a provided key or function, and returns a map of the grouped items. The `groupByKey()` function allows for grouping of list items based on the value of a specific key in each item, and also returns a map of the grouped items.
- The `latest()` function returns the most recent item in the list based on a provided key or function, while the `latestFirst()` function sorts the list in descending order based on the provided key or function.
- The `oldest()` function returns the oldest item in the list based on a provided key or function, while the `oldestFirst()` function sorts the list in ascending order based on the provided key or function.

### Changed

- Changed `sortByDesc()` to `sortDescBy()` in list extension

## 2.0.0

### Braking Changes

- Added `append()` and `prepend()` string extension.
- Added `flatten` and `pluck()` list extension.
- Changed `w` to` wBox` and `h` to `hBox` in num extension.
- Changed `range` to `inRange` in String extension.
- Changed `count` to `occurrences` in String extension.
- Changed `occurrence` to `countOccurrences` in String extension.
- Changed `withDefault` to `ifEmpty` in String extension.
- Changed `getId` data type from dynamic to int in map extension.
- Changed `contains` to `has` in map extension.
- Fixed `mask` now return `null` when string is empty.
- Fixed `getInt` & `getDouble` now return `null` when key is empty or null.
- Fixed Typo

## 1.7.0

### Added

- Added `black` and `white` color
- Added `context` extension on Build Context
- Added Responsive extension

### Changed

- changed `.h` & `.w` child widget to optional in num extension
- changed `.maxLine` to optional in Text extension
- changed `.box` to `.sq` in num extension

## 1.6.0

### Added

- Added `match()` extension on `Map`

  The `match()` function also works similarly to `switch`
  i.e, it finds the matching case according to the parameter passed in it.

- Added `hasKey` | `hasValue` | `hasKeyValue` extensions on list

## 1.5.0

### Added

- Write tests for `List`
- Write tests for `Map`

### Changed

- Changed `.textScaleFactor` => `.textScale`
- Changed `.fs` => `.fontSize`
- Removed `isEmptyOrNull` & `isNotEmptyOrNull`

## 1.4.0

### Added

- Added `random` | `chunk` | `split` list extensions

### Fixed

- Fixed `sortBy` error when list doesn't have this key or it doesn't have list of map

## 1.3.0

### Added

- Added `sq` | `w` | `h` num and widget extensions
- Added `Duration` num extensions like `seconds` | `minutes`, etc

## 1.2.0

### Added

- Added `suffix` num extensions
- Added `getMonthName` & `getWeekName` int extensions

### Fixed

- Fix Text color extensions.
- Fix `isUpper` & `isLower` String extensions
- Fix `hideIf` & `showIf` Widget extensions

## 1.1.0

### Added

- Added `sortBy()` , `sortByDesc()` in List.

### Fixed

- Fix Text heading.

## 1.0.0

- Initial release.
