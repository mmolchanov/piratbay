# Semantic Layer: request_volume_fact

## Dimensions

- business
- request_type
- desk
- sub_desk
- analyst
- manager
- salesperson
- region
- desk_location
- cash_vs_deriv
- status

## Date dimensions

- request_date
- completed_date
- cancelled_date
- in_progress_date
- on_hold_date

## Measures

- Request Count = count of `request_id` where `received_flag = 1`
- Completed Requests = count of `request_id` where `completed_flag = 1`
- Cancelled Requests = count of `request_id` where `cancelled_flag = 1`
- In Progress Requests = count of `request_id` where `in_progress_flag = 1`
- On Hold Requests = count of `request_id` where `on_hold_flag = 1`

## Calendar logic

`period_month` and `period_year` are common calendar concepts derived dynamically from the relevant status date. For received requests they map to `request_date`; for completed requests they map to `completed_date`; for cancelled requests they map to `cancelled_date`; for in-progress requests they map to `in_progress_date`; for on-hold requests they map to `on_hold_date`.
