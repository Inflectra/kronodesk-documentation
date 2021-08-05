# Release Notes for KronoDesk v1

## Version 1.1 (October 2013)

!!! success "New features"

    - Users can upload small graphic avatars that will be displayed in forums and help desk
    - Users can specify override timezone and culture
    - Display forum statistics and total number open/answered messages in each forum
    - Support for meta-tags in Forums with Tag Cloud for easy access to tagged threads
    - Workflow step/status can be marked separately as 'active' for submitter and 'active' for agent
    - Templating system for all help desk notifications and emails
    - Customizable Reporting system including graphs, data-grids and MS-Excel, CSV exports
    - Mobile web interface for Apple iOS Devices and Android Devices
    - Enhanced ability to change look and feel of application to match company standards / website
    - REST Web Services API added in addition to existing SOAP Web Services API

!!! bug "Bug fixes and enhancements"

    - Ability for system to 'auto-close' after a period of time.
    - Fixes issue that prevents articles being created when system installed on a server configured for UTC+X timezones
    - Fixes issue where deleting existing custom properties in Administration doesn’t do anything
    - Stores user settings in database so that the system remembers filters, opened/closed widgets, etc.
    - Fixes issue where some forum email messages were leaving the ${…} tokens in the final message
    - My Subscribed Articles widget added to both customer and employee dashboards
    - Closed date now auto-populates and clears when you close/open a help desk ticket
    - Bug when searching users by full name in the administration section is fixed
    - Watermark added to the ticket creation page to better explain to customers the purpose of the Ticket Name field