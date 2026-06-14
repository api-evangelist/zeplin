# Zeplin GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the Zeplin design handoff and collaboration platform. Zeplin bridges designers and developers by providing structured access to design specs, assets, style guides, components, and annotations exported from Figma, Sketch, and Adobe XD.

The schema is derived from the Zeplin REST API (https://docs.zeplin.dev/reference/) and models the full surface area of the platform including projects, screens, components, style guides, design tokens, members, webhooks, comments, and activity.

## Source

- REST API Reference: https://docs.zeplin.dev/reference/
- OpenAPI Spec: https://github.com/zeplin/openapi
- Authentication: OAuth 2.0 with PKCE, personal access tokens

## Schema File

See `zeplin-schema.graphql` for the full type definitions.

## Types Summary

### Projects and Screens
- `Project` / `ProjectDetails` — top-level design project containers
- `ProjectType` — enum distinguishing project kinds (web, iOS, Android, macOS)
- `ProjectStatus` — active, archived states
- `ProjectSection` — organizational groupings within a project
- `Screen` / `ScreenDetails` — individual design screens/artboards
- `ScreenVersion` — historical versions of a screen
- `ScreenNote` — annotations attached to a screen
- `ScreenSection` — grouping of screens within a project
- `ScreenTag` — labels applied to screens

### Layers
- `Layer` — base design layer (rectangle, text, image, group, component)
- `LayerGroup` — container grouping multiple layers
- `TextLayer` — layer with typographic content and text styles
- `ShapeLayer` — vector or fill-based shape layer

### Components
- `Component` / `ComponentDetails` — reusable design component
- `ComponentSection` — grouping of components within a styleguide or project

### Style Guides and Design Tokens
- `StyleGuide` / `StyleGuideDetails` — shared design system resource
- `StyleGuideSection` — section within a style guide
- `Color` / `ColorSwatch` — named colors and swatches
- `PaletteGroup` — grouped set of color swatches
- `TextStyle` / `TextStyleGroup` — typographic styles
- `Typography` — typography configuration (font, size, weight, line-height)
- `Spacing` / `SpacingSection` — spacing tokens and their groupings
- `Grid` / `GridDetails` — layout grid specifications

### Assets
- `Asset` — exportable design asset
- `AssetExport` — export configuration for an asset
- `AssetFormat` — file format enum (PNG, JPG, SVG, PDF, WEBP)
- `DensityScale` — pixel density multiplier (1x, 2x, 3x)
- `AssetResolution` — explicit resolution override

### Members and Permissions
- `Member` — a user participating in a project or organization
- `MemberRole` — role enum (owner, admin, editor, viewer)
- `Permission` — fine-grained capability flag
- `Organization` / `OrganizationDetails` — workspace-level grouping
- `OrganizationMember` — member of an organization
- `Invitation` — pending invite to join a project or organization

### Webhooks and Integrations
- `Webhook` — webhook subscription configuration
- `WebhookEvent` — enum of event types that can trigger webhooks

### Collaboration
- `Comment` — threaded comment on a screen or layer
- `Note` — standalone annotation on a design artifact
- `ActivityFeed` — stream of activity events across a project

### Authentication
- `APIKey` — personal access token for API authentication
- `Token` — OAuth token response

## Usage

This conceptual GraphQL schema can be used to:

1. Build a GraphQL gateway or BFF (backend for frontend) over the Zeplin REST API
2. Understand the data model and relationships in Zeplin
3. Generate type-safe client code for design tooling integrations
4. Train AI models on Zeplin's domain concepts

## Notes

Zeplin does not currently expose a native GraphQL endpoint. This schema represents a faithful mapping of the REST API surface into GraphQL idioms, preserving relationships and field names as closely as possible.
