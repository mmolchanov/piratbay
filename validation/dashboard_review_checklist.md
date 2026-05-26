# Dashboard Review Checklist

- Uses only columns from `request_volume_fact`.
- Does not invent unavailable measures or dimensions.
- Includes start date and end date filters.
- Excludes Cycle Times section.
- Excludes Cancelations section.
- Treats `desk_location` as city-level data.
- Treats `analyst`, `manager`, and `salesperson` as full-name dimensions.
- Uses status-specific dates for status metrics.
- Produces stable layout and naming from run to run.
