# Content Marketplace

Content marketplace for apps containing dashboards, rules, notebooks, presets, and datasets.

## Structure

- `template_app/` - Example app structure showing all content types
- `schema/` - JSON schemas for validation (`appIndex.schema.yaml`, `dashboard.schema.yaml`, etc.)

## App Structure

Each app requires:
- `appIndex.yaml` - App metadata (see `schema/appIndex.schema.yaml`)
- `appIcon.png` - App icon
- `version.yaml` - Version history (see `schema/version.schema.yaml`)

Content types (at least one required):
- `dashboards/` - Dashboard definitions with optional screenshots
- `rules/` - Detection rules (YAML)
- `notebooks/` - Databricks notebooks (.ipynb)
- `presets/` - Preset configurations
- `datasets/` - Local or remote datasets (CSV/JSON)

Each content directory can have a `revisions.yaml` for version tracking.

See `template_app/` for a complete example.
