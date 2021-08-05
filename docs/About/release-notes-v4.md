# Release Notes for KronoDesk v4

## Version 4.0 (August 2021)

!!! info "Summary"
    - Adds Active Directory / LDAP support for user creation and authentication, giving on premise customers an alternate way to manage user authentication
    - Brand [new installer](../../Administration-Guide/Installing-KronoDesk) for on premise customers with enhanced functionality and a streamlined user interface

!!! success "New features"
    - Rebuild and upgrade the [on-premise installer application](../../Administration-Guide/Installing-KronoDesk) to improved functionality and usability [RQ:2389]

    * **Active Directory / LDAP support for user creation and authentication**

        - Add system administration LDAP Configuration Page [RQ:3504]
        - Add the ability to import users from LDAP via new dedicated system admin pages [RQ:3505]
        - Admin Edit User Details Page lets admins view, edit, add, and remove LDAP settings for a user [RQ:3506]


!!! bug "Bug fixes and enhancements"
    - Fix deleting a custom list or value in use by a custom property throwing an error on the ticket details page [IN:2655]
    - Ensure that only logged in internal users can access the API documentation pages [IN:3058]
    - Improve the language of the action buttons on the article (KB) edit page to make their meaning clearer [IN:3982]
    - Ensure that tooltips on the Help Desk ticket list table always show the the latest note to internal users [IN:3990]
    - Allow system administrators to change the [login ID](../../Administration-Guide/Users/#manage-users) of existing users [IN:4353]
    - Move the activity indicator icon to the left so that it does not obscure the user icon [IN:4888]
    - Fix the Recent Forum Posts widget on the home page sometimes displaying the entire forum post [IN:4918]
    - Fix changes not being saved on the organization detail page if the organization name is less than 5 characters [IN:5029]
    - Fix the display of the ticket name on the help desk ticket list page, so names are not cut off if they contain a "&" character [IN:5070]
    - Remove headers for deactivated sections showing on the external home page [IN:5279]
    - Improve how merging tickets works so each ticket becomes a distinct note on the combined ticket (merging no longer merges descriptions together) [IN:5288]
    - Fix the help desk ticket list table tooltip not properly displaying due to not escaping quote characters [IN:5308]
    - Fix user profile showing January 1, 0001 as the Member Since date for some users [IN:6210]
    - Internal links to documentation point to KronoDocs website instead of internal help files [IN:6225]
    - Fix clicking on tickets created by a user who is currently inactive displaying a system error [IN:6236]
    - Fix the global search returning inaccurate information under certain circumstances [IN:6248]
    - Remove headers for deactivated areas on the user profile page [IN:6249]
    - Fix searching for tickets within an organization showing an error [IN:6250]
    - Fix the ticket section of the external home page being blank if the Knowledge Base and/or Forum sections are disabled [IN:6478]
    - Improve the styling and display of error pages [IN:6548]
    - Ensure new installations create the database with the setting AUTO_CLOSE = False [IN:6568]
    - Make the language on the administration email menu option consistent with the heading on the Email Options page [IN:6585]
    - Improve the summary message on the administration > System Settings > Orphaned Documents page to make it more clear [IN:6586]
    - Remove the double colons from certain labels on the administration > Users > Security page [IN:6587]
    - Improve the message text on the administration > Users > User Roles page to make it more clear [IN:6588]
    - Fix spelling errors on the administration > Forum Settings > Appearance page [IN:6589]
    - Security fixes
