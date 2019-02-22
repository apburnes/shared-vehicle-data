shared-vehicle-data
===================

Static data files collected from shared vehicle systems

## Contents

- `dc/`
    - Shared vehicle data from Washington DC
    - Snapshots are requested every 15 minutes
    - Collection date range from December 2018 to February 2019

    - `ff-dow-hourly-grouping/`
        - These are free floating shared vehicles *(dockless bikes and scooters)* that are grouped by the numeric day of the week *(1-7)* and the hour *(0-23)*
        - Each grouping is exported into a csv file
        - Data Fields
            - `vehicle_id`:
                - type: **string**
                - description: Vehicle unique identifier
            - `name`:
                - type: **string**
                - description: Vehicle name
            - `last_reported`:
                - type: **date**
                - timezone: **US/Eastern**
            - `system_id`:
                - type: **string**
                - description: Name of the shared vehicle provider
            - `vehicle_type`:
                - type: **string**
                - choices: **manual-bike** or **pedal-assist-bike** or **electric-scooter**
            - `collected_at`:
                - type: **date**
                - timezone: **US/Eastern**
            - `lon`:
                - type: **number**
                - description: Vehicle location longitude
            - `lat`:
                - type: **number**
                - description: Vehicle location latitude

