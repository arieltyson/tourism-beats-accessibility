# Tourism Beats Accessibility

**Last updated:** March 2026

Tourism Beats is designed to make city discovery, travel planning, and food journaling more accessible to more people over time. This page documents the app's current accessibility support and the work in progress behind Tourism Beats' Accessibility Nutrition Labels for App Store Connect.

The summary below reflects the current iPhone experience for the main user flows in the app:

- browsing featured cities and searching destinations
- reading city details, weather, local time, and advisories
- using the music, food journal, and trips experiences
- creating and editing restaurants, trips, and trip activities

## Nutrition Label Summary

| Feature | Status | Notes |
|---|---|---|
| **VoiceOver** | In progress | Standard controls, grouped cards, and many primary surfaces are labeled. Final end-to-end validation is still in progress for custom exploration flows like the map and city pager. |
| **Voice Control** | In progress | Most actions use standard SwiftUI controls with visible labels. Custom map and gesture-driven navigation are still under final validation. |
| **Larger Text** | In progress | Dynamic Type support has been improved across common tasks, including time, city facts, walkability, and picker/search surfaces. Final largest-size device testing is still in progress. |
| **Dark Interface** | Fully supported | Core surfaces, glass cards, and semantic colors support Light and Dark appearance across the app. |
| **Sufficient Contrast** | In progress | The semantic color system adapts for higher contrast, but some image- and glass-heavy screens are still being refined and verified. |
| **Differentiate Without Color** | In progress | Many travel, visa, safety, restaurant, and trip states already use text or symbols in addition to color. A full audit of every color-coded state is still underway. |
| **Reduce Motion** | In progress | Major common-task animations now reduce or disable when Reduce Motion is enabled. A final sweep is still underway to verify every remaining transition and decorative effect. |
| **Closed Captions** | Not applicable | Tourism Beats does not currently contain video or audio-only content with dialogue that requires timed captions. |
| **Audio Descriptions** | Not applicable | Tourism Beats does not currently contain video content that requires audio descriptions. |

## VoiceOver

Tourism Beats already includes meaningful VoiceOver support in several primary areas:

- **Home** — featured destination cards and the main Explore call to action expose descriptive labels and hints.
- **Food Journal** — city cards, restaurant cards, and score controls provide grouped labels and accessible values.
- **Trips** — trip cards and major actions expose combined labels and summaries.
- **Advisories** — hero, safety, visa, and walkability cards expose grouped content instead of forcing users to navigate every decorative subview.

Current focus areas still being validated:

- **Map exploration** — Tourism Beats uses a native `MKMapView` bridge for destination discovery, and this flow is still being manually audited with VoiceOver.
- **City page switching** — the app provides an accessible page indicator, but the custom vertical paging container is still being tested end to end.
- **Complex edit flows** — trip, activity, and restaurant forms are accessible, but the final VoiceOver pass is still in progress for every sheet and edge case.

## Voice Control

Tourism Beats leans heavily on standard SwiftUI controls, which provides a strong baseline for Voice Control:

- buttons, menus, pickers, date pickers, toggles, alerts, sheets, navigation links, and text fields use native controls
- high-traffic actions such as **Create Trip**, **Add Restaurant**, **Filter trips**, **Filter restaurants**, **Edit**, and **Delete** expose visible text or system labels
- segmented controls are used for core filters and statuses instead of custom gesture-only controls

The main Voice Control validation still in progress is around custom navigation experiences:

- **destination map selection**
- **vertical city-page switching**

## Larger Text & Dynamic Type

Tourism Beats has been updated to better support the largest accessibility text sizes:

- all major text styles use scalable system typography tokens
- the **local time** card now switches to a text-first accessibility layout at accessibility Dynamic Type sizes
- the **city fun fact** card no longer relies on a fixed-height layout when text is larger
- **walkability scores** now use scalable typography instead of a fixed point size
- **country picker** section indexing is hidden at accessibility sizes to preserve readability and avoid crowding
- search-result highlighting no longer forces a fixed-size font

Final validation is still in progress at the very largest sizes to confirm:

- no clipping in every city detail state
- no truncation in music and hero-card overlays
- comfortable edit-flow usability in the food and trips sheets

## Dark Interface

Tourism Beats fully supports Dark Interface today:

- semantic brand, status, surface, and label colors resolve for both Light and Dark appearance
- glass cards automatically fall back to solid surfaces when Reduce Transparency is enabled
- map exploration uses a dark map presentation
- the app's main presentation style, image-backed cards, and elevated surfaces are designed around dark-friendly contrast and materials

## Sufficient Contrast

Tourism Beats includes a contrast-adaptive semantic color system and supports higher-contrast variants for its core brand and status colors. This work covers:

- primary semantic colors for safe, caution, danger, and informational states
- adaptive main surfaces and secondary surfaces
- readable primary and secondary label colors across light and dark appearances

Work still in progress:

- verifying contrast on image-backed hero cards
- strengthening text treatment on some glass and media surfaces
- completing the full screen-by-screen audit with **Increase Contrast** enabled

## Differentiate Without Color

Tourism Beats already uses more than color in many places:

- visa states use iconography and text
- safety and walkability summaries use labels, scores, and descriptive copy
- restaurant and trip states use text, symbols, and layout grouping in addition to color
- selected page states and filter states include icon changes or selection traits

The remaining work is a full audit to ensure every information-bearing state stays clear without relying on color alone, especially in decorative or highly visual card layouts.

## Reduce Motion

Tourism Beats has recently expanded its Reduce Motion behavior across common tasks:

- **Food** and **Trips** empty states no longer pulse when Reduce Motion is enabled
- filter icons in the food and trips toolbars no longer bounce when Reduce Motion is enabled
- city-page transitions and advisory-card entrance effects now degrade to low- or no-motion variants
- weather and fact card transitions now use reduced-motion-aware animation handling
- form toggles and restaurant score interactions now avoid unnecessary motion for reduced-motion users
- the analog clock stops using spring motion when Reduce Motion is enabled

Final verification is still in progress for every remaining decorative or secondary animation in the app.

## Testing

Tourism Beats is being audited against Apple's Accessibility Nutrition Label categories using common-task-based validation, including:

- featured destination browsing
- search and city selection
- city detail reading
- advisory review
- music actions
- food journal entry and editing
- trip planning, editing, and deletion

The app's accessibility statement and App Store Connect responses will continue to be updated as the audit is completed and additional fixes ship.

## Contact

If you have questions or feedback about Tourism Beats accessibility, please contact us at arieltyson30190@gmail.com.
