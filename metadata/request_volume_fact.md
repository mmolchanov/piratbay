# request_volume_fact Metadata

## Grain
One row represents one BI request.

## Columns

| Column | Description |
|---|---|
| request_id | Unique request identifier. |
| business | Business area. |
| request_date | Date when the request was received. |
| completed_date | Date when the request was completed. |
| cancelled_date | Date when the request was cancelled. |
| in_progress_date | Date when the request moved to in progress. |
| on_hold_date | Date when the request moved to on hold. |
| status | Current request status. |
| request_type | Type of BI request. |
| desk | Desk category. |
| sub_desk | Desk sub-category. |
| analyst | Analyst full name. |
| manager | Analyst manager full name. |
| salesperson | Salesperson full name. |
| region | Geographic region. |
| desk_location | City-level desk location. |
| cash_vs_deriv | Cash or derivative indicator. |
| received_flag | 1 when request is counted as received. |
| completed_flag | 1 when request is counted as completed. |
| cancelled_flag | 1 when request is counted as cancelled. |
| in_progress_flag | 1 when request is counted as in progress. |
| on_hold_flag | 1 when request is counted as on hold. |

## Date logic
Use the event-specific date for each status metric. Received uses `request_date`, completed uses `completed_date`, cancelled uses `cancelled_date`, in progress uses `in_progress_date`, and on hold uses `on_hold_date`.
