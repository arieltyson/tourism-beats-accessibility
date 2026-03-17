# Tourism Beats Accessibility

**Last updated:** March 16, 2026

Tourism Beats is an iPhone app for destination discovery, local travel research, food journaling, and trip planning. This page documents the app's current accessibility support for the common tasks users complete in Tourism Beats and supports the app's Accessibility Nutrition Labels in App Store Connect.

This statement currently covers the **iPhone** experience.

## Common Tasks Covered

The accessibility support described on this page applies to the app's primary common tasks, including:

- browsing featured cities and searching destinations
- opening a city and reading time, weather, music, and advisory information
- exploring the destination map and switching between city detail sections
- browsing the food journal, opening a city, and adding or editing restaurants
- creating, editing, and deleting trips, days, and trip activities
- reviewing visa, safety, and walkability information

## Nutrition Label Summary

| Feature | Status | Notes |
|---|---|---|
| **VoiceOver** | Supported on iPhone | Tourism Beats uses accessible labels, values, hints, grouped content, and adjustable navigation for common tasks across city discovery, food journaling, and trip planning. |
| **Voice Control** | Supported on iPhone | Core actions use native controls with visible text or discoverable accessibility input labels, including map, food, and trip interactions. |
| **Larger Text** | Supported on iPhone | Core layouts scale with Dynamic Type, including city detail cards, picker/search surfaces, food cards, and trip planning flows. |
| **Dark Interface** | Fully supported on iPhone | Tourism Beats supports Light and Dark appearance with semantic surfaces, adaptive labels, and dark-friendly imagery treatments. |
| **Differentiate Without Color Alone** | Supported on iPhone | Key states use text, symbols, labels, layout, or badges in addition to color across advisories, food, and trips. |
| **Sufficient Contrast** | Supported on iPhone | The app uses adaptive semantic colors, stronger image scrims, and higher-contrast variants for text and controls across common tasks. |
| **Reduced Motion** | Supported on iPhone | Motion-heavy effects are reduced or disabled for common tasks when Reduce Motion is enabled. |
| **Closed Captions** | Not applicable | Tourism Beats does not currently provide video or audio-only content with dialogue that requires timed captions. |
| **Audio Descriptions** | Not applicable | Tourism Beats does not currently provide video content that requires audio descriptions. |

## VoiceOver

Tourism Beats supports VoiceOver for the app's common tasks on iPhone.

Current support includes:

- descriptive labels, values, and hints for featured destination cards, search results, and city detail entry points
- grouped accessibility content for weather, food, restaurant, and trip summary cards
- accessible edit flows for trips, trip activities, and restaurants
- accessible status, score, and badge summaries for food journaling and trip planning
- an adjustable city section indicator so users can move between **City**, **Music**, and **Advisories**
- clearer map semantics and full destination titles for map-based discovery

## Voice Control

Tourism Beats supports Voice Control for the app's common tasks on iPhone.

This support is based on:

- broad use of native SwiftUI controls such as buttons, menus, pickers, toggles, alerts, sheets, and text fields
- visible text labels for primary actions like **Create Trip**, **Add Restaurant**, **Edit**, **Delete**, **Save**, and **Filter**
- accessibility input labels on high-traffic controls in the food, trip, and destination-detail flows
- native map and navigation surfaces that remain reachable without custom gesture-only interaction requirements

## Larger Text

Tourism Beats supports Larger Text on iPhone for its common tasks.

The app uses scalable system typography and adaptive layouts across the product, including:

- local time, weather, and city fact presentation
- search and country-selection surfaces
- food city cards and restaurant cards
- trip overview cards, trip detail summaries, and trip planning forms
- walkability and advisory summaries

Large-text improvements include reflowing content, avoiding fixed-size text in core views, and relaxing truncation in card-based interfaces where larger text sizes need more room.

## Dark Interface

Tourism Beats fully supports Dark Interface on iPhone.

This includes:

- semantic surface and label colors that resolve correctly in Light and Dark appearance
- dark-friendly card treatments for image-backed, glass, and elevated surfaces
- adaptive materials and fallback surfaces for readability
- consistent presentation across discovery, city detail, food, and trips flows

## Differentiate Without Color Alone

Tourism Beats supports Differentiate Without Color Alone on iPhone.

Across common tasks, the app uses more than color to communicate important state:

- text labels and iconography on visa, safety, and walkability surfaces
- visible labels and status copy on restaurant, trip, and activity states
- badges, symbols, and layout grouping for selection and progress states
- page and filter states that remain understandable without relying on tint alone

## Sufficient Contrast

Tourism Beats supports Sufficient Contrast on iPhone.

The app uses:

- semantic label and surface colors that adapt for readability
- stronger image scrims and badge fills on image-backed cards
- adaptive contrast-aware color tokens for primary content, secondary content, and controls
- higher-contrast handling across city detail, food journal, and trips surfaces

## Reduced Motion

Tourism Beats supports Reduced Motion on iPhone.

When Reduce Motion is enabled, the app reduces or disables motion-heavy effects in common tasks, including:

- pulsing or bouncing empty-state and filter affordances
- city detail and advisory transition effects
- food and trip card animation behavior
- fact, weather, and page transition animations
- spring-heavy clock and form interaction motion

## Media Accessibility

Tourism Beats does not currently include timed media experiences that require Accessibility Nutrition Label support for captions or audio descriptions.

- **Closed Captions:** not applicable
- **Audio Descriptions:** not applicable

## Ongoing Accessibility Work

Accessibility is an ongoing part of Tourism Beats development. As the app evolves, this page will be updated to reflect new accessibility improvements, additional testing, and any changes to the app's common-task support.

## Contact

If you have questions or feedback about Tourism Beats accessibility, please contact arieltyson30190@gmail.com.
