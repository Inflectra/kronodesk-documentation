# Release Notes for KronoDesk v3

## Version 3.0 (January 2019)

!!! success "New features"

    - Customization

        - Admins can enable/disable Ticket fields. [RQ:2271]

    - Reporting

        - Ability to Generate Standard Reports [RQ:1463]

    - Ticket Details page is fast, responsive, easy to use, and intuitive

        - A journal view lets users easily see, understand, and act on all aspects of the ticket history [RQ:2268]
        - Ticket header displays clear standard information that is easy to act on [RQ:2285]
        - New sidebar shows rich information about a user, and gives access to all custom fields [RQ:2286]
        - Digital Signatures makes uses sign when workflow requires it [RQ:2287]
        - Attachments can be easily added (and subsequently managed) on a ticket [RQ:2288]
        - Incidents to SpiraTeam can be created, when applicable [RQ:2289]
        - Workflow management and field validation is easy to use and gives clear feedback to user [RQ:2290]
        - Save buttons gives clear signposts and actions to user [RQ:2294]
        - The page is responsive and usable at all screen sizes [RQ:2291]
        - Ticket Details has live reloading [RQ:2297]
        - Keyboard shortcuts make using the page quicker and possible without a mouse [RQ:2350]
        - Users can see and change cc members to a ticket [RQ:2353]
        - Employee Groups [RQ:2372]
        - Ticket Create Page: is fast, responsive, and easy to use [RQ:2355]
        - Ticket details organization roles control permissions in correct sync with workflow [RQ:2379]
        - KB articles are easier to read [RQ:2354]
        - Refactoring KB pages [RQ:2356]
        - Create API for v3.0 [RQ:2370]
        - Refactoring [RQ:2371]
        - allow admins to customize js loaded on the site [RQ:2373]
        - Add Undelete button for internal users [RQ:2388]


!!! bug "Bug fixes and enhancements"

    - Report Types [IN:2360]
    - Ability to report on companies and users belonging to. [IN:2374]
    - Subscribed Threads widget: show last updated date instead of the date the thread was created [IN:2609]
    - Ability to have a CC list associated with a ticket [IN:2805]
    - Add print screen option to KB articles. [IN:3491]
    - Creating an incident in Spira: required custom property is not enforced. [IN:3949]
    - CSRF in Able To Reply Anything Of Any Post Without Victim Permission [IN:3965]
    - Administration -> Knowledge Base settings: various problems trying to set up categories [IN:4016]
    - Add 'User Merge' Functionality [IN:4110]
    - Implement CSP Policy on KronoDesk [IN:4157]
    - Disconnect between DataGridJ and filterHtml() function. [IN:4213]
    - Store Attachment URLs as tokens, to be translated upon display. [IN:4220]
    - When attempting to view an attachment that is not accessible, a system error is displayed. [IN:4241]
    - Upgrade from 2.0 to 2.1: error editing the sample organizations [IN:4243]
    - Documentation: add info about "Log In As User" button to the admin manual. [IN:4322]
    - Forum posts: after 24 hours, the time is 5 hours later than it should be. [IN:4323]
    - Issues with forum posts from user who has been made inactive [IN:4324]
    - XSS vulnerability submitting new ticket [IN:4469]
    - Enhancement - Add ability to print single Ticket [IN:4574]
    - System error trying to view user profile if login ends with a period [IN:4748]
    - Make the experience better when trying to create a ticket before authenticated [IN:4783]