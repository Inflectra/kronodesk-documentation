# Release Notes for KronoDesk v2

## Version 2.1 (September 2017)

!!! success "New Features"

    - Organization Management
    
        - Ability to group external users that belong to one customer organization [RQ:1724]
        - Ability to see all of the tickets in this organization group [RQ:1872]
    
    - Improve the Administration main menu [RQ:1917]
    - Support for Electronic/Digital Signatures of Transitions [RQ:2101]
    - Support for Digital Signatures [RQ:2119]
    - Rewriting the graphs in KronoDesk in C3/D3 [RQ:2122]
    - Ability to export the history grid to CSV [RQ:2141]

!!! bug "Bug fixes and enhancements"

    - Add option to disable user creation. [IN:2052]
    - Approveal of new user [IN:2334]
    - Changing of Opener and Private custom properties [IN:2343]
    - When you save a graph as a JPG, BMP or PNG, the result has no labels or key. [IN:2596]
    - Ticket detail page, Add New Incident dialog: add the ability to move and resize the window [IN:2963]
    - Add CAPTCHAs to prevent automation of forms [IN:3049]
    - No Email Verification after Registration [IN:3059]
    - Deleting user forgot a Foreign Link [IN:3201]
    - Admin Edit User & New User, and User's Profile pages are identical - Combine them. [IN:3698]
    - Article tag cloud should only show top 25 tags [IN:3844]
    - Add history refresh button to ticket detail page [IN:3866]
    - Weird dialog box when you try to assign ticket via. context menu [IN:3931]
    - The ticket URLs are showing double slashes on the ticket details page nav bar [IN:3938]
    - Replying to a forum thread: confusing behavior if you select subscribe when you are already subscribed [IN:3939]
    - Ticket details - move scrollbar to the right edge of the page [IN:3956]
    - On Gallifrey (freshly installed system), there are no avatars included with the sample users [IN:3964]
    - On certain pages, it's really really difficult to select from dropdown lists [IN:3967]
    - Save & Revert Buttons on Forum FAQ [IN:3969]
    - Forum Guidelines Save button missing on MS Edge and Chrome (Firefox OK) [IN:3973]
    - Bug when someone deletes a custom property. [IN:3997]
    - Ticket list: if you have rearranged the columns, the pop-up for showing and hiding columns is very confusing [IN:3998]
    - Help desk ticket tool tips: time is off by 4 hours. [IN:4002]
    - Add incident to Spira Popup does not display properly on Safari on MD screens [IN:4007]
    - Administration -> Knowledge Base settings: various problems trying to set up categories [IN:4016]
    - XSS Bug on User Profile if thread/reply has javascript encoded [IN:4049]
    - Ticket details: Make error message visible, even if you have scrolled down. [IN:4076]
    - Ticket detail page: in Chrome, there's no pop-up to warn you of unsaved changes [IN:4077]
    - Tooltips prevent some dropdowns from being selected [IN:4082]
    - External Home Page Help Desk description does not change based on KB/forum turned on or not [IN:4091]
    - Draft KB article is found by searching [IN:4095]
    - KB and Forum appear in navbar, when turned off in admin, and user not logged in [IN:4097]
    - Help Desk custom properties: sometimes, the Edit Definition button does not work [IN:4103]
    - Stored XSS Vulnerability on Account Login name [IN:4138]
    - Regarding Critical Stored XSS Vulnerability at Inflectra Support [IN:4144]
    - We have a Stored XSS issue on the Admin - User List Page [IN:4185]
    - Invalid License page not stylized [IN:4221]
    - Installation issue: online help is formatted incorrectly. [IN:4227]
    - Admin manual is missing the new user security options [IN:4231]
    - Upgrade from 2.0 to 2.1: organization roles are labeled incorrectly [IN:4235]
    - Verifying account: email address is filled in correctly at first, but goes blank if other invalid data is entered... [IN:4236]
    - Organization list page: # users column is always blank [IN:4239]


## Version 2.0 (February 2017)

!!! success "New features"

    * **Role Management**

        - Create, modify and delete roles [RQ:1135]
        - Customizable role permissions [RQ:968]

    * **Help Desk Ticketing**

        -  Auto-suggest KB article when customer submitting ticket [RQ:1756]
        -  Ability for support agents to seamlessly enter a KB link into tickets [RQ:1757]
        -  Option to email attached document to ticket submitter when attaching [RQ:1414]

    * **Knowledge Base**

        -  RSS Feed for recent articles [RQ:1174]
        -  Each category has a page with its articles [RQ:1149]
        -  RSS Feed for each category page [RQ:1150]
        -  Separate Links Panel for KB Article [RQ:1883]

    * Replacement of separate mobile site with a single adaptive site [RQ:1826]
    * Refresh of KronoDesk UI to be more modern looking [RQ:1827]
    * Improved Global Search [RQ:1881]
    * Integrated Theming [RQ:1882]
    * Create new v2.0 REST API and SOAP API [RQ:1884]
    * Update Incidents Logging for Spira 5.0 [RQ:1885]


!!! bug "Bug fixes and enhancements"

    - Allow option to send Email Attachments in notification. [IN:1993]
    - Allow merging of tickets. [IN:2134]
    - Make it easier to see and/or copy the contents of the description field [IN:2259]
    - Help Desk: error when trying to change to a view that only has one page, while currently on a subsequent page [IN:2264]
    - Forum heading "Last Post" information is incorrect, if there are any new threads that are newer than the last thread REPLY [IN:2305]
    - Help Desk: Filtering by date has problems [IN:2393]
    - Help desk ticket list: allow users to customize the list display and remember their choices. [IN:2470]
    - Administration>Ticket Statuses page: Add a warning/confirmation message when user clicks on "remove". [IN:2505]
    - Help Desk, Ticket detail page: the display dropdown options on the left don't work as expected for customers [IN:2520]
    - Administration > System Settings > E-Mail Configuration page: one of the tabs isn't displaying right, plus some suggestions for making it easier to understand: [IN:2525]
    - Help Desk: Ticket "Closed Date" field always gets populated when you revert a workflow transition. [IN:2548]
    - Help Desk ticket list: There's no way to get back to sorting by last updated, if you choose a different sort [IN:2565]
    - global search results box can disappear if you move the mouse [IN:2569]
    - In the ticket description, indicate that a note is internal only. (was done for the notes section already) [IN:2576]
    - In one forum screen, avatars aren't scaled down like they are on other screens. [IN:2577]
    - With Firefox, the screen for submitting a ticket is too wide [IN:2580]
    - Add Option to remove email header line. [IN:2582]
    - Help desk: Name and Product fields are always required even if the workflow doesn't have the "required" box checked. [IN:2587]
    - Add security roles to application sections. [IN:2594]
    - Don't trigger Event Notifications when an internal note is added [IN:2595]
    - Admin editing users can select 'no' roles, throwing error. [IN:2599]
    - Help desk ticket history problem if there is more than one page of history: can't go to subsequent page(s) [IN:2603]
    - Company information not displaying properly [IN:2607]
    - Add KronoDesk ticket link to Spira [IN:2650]
    - Description heading missing on the New Ticket screen [IN:2673]
    - kronos- user view vs employee view [IN:2676]
    - overview of my logged tickets. Allow customers to export their tickets to Excel. [IN:2693]
    - Add ability to configure additional roles [IN:2743]
    - Help desk: Long lines in the Error Message field don't wrap, thus causing the whole screen to be too wide [IN:2744]
    - Having a custom property of type integer doesn't validate safely if a user enters a non-integer. [IN:2750]
    - Creating an incident in SpiraTeam works, but a strange error is logged. [IN:2756]
    - Minor labeling problem with the Ticket Date Range graphs: data grid always shows "Ticket Progress Rate" label. . . [IN:2757]
    - Ticket history table won't let you view more than one page. [IN:2847]
    - Improper UserCollection entry causing a NullReferenceExcpetion in Ticket_Retrieve() [IN:2848]
    - User list in Administration can get into a state where it cannot be displayed. [IN:2849]
    - Email Config Page doesn't inactivate IIS SMTP setting when hosted. [IN:2862]
    - Allow employees to view their own attachments before tickets submittted [IN:2876]
    - Sporadic Width Issues Submitting Tickets on Chrome [IN:2960]
    - Help Desk: ticket page has display problem on wide screens [IN:2962]
    - Help Desk: on New Ticket page, make the ticket name field more noticeable somehow [IN:2965]
    - Dropdowns on the ticket detail page are hard to use [IN:2966]
    - permission/membership issues when adding an incident to Spira [IN:2967]
    - KronoDesk priority colors customizable [IN:3016]
    - Kronodesk footers: disable [IN:3022]
    - Dropdowns don't always select all items (those near the end remain unselected) [IN:3039]
    - Insufficient Security Validation of User-supplied Input – Path Traversal [IN:3050]
    - Login Name Input Validation Only Enforced Client Side [IN:3051]
    - Prevent Display of Attachments Linked to Tickets by Anonymous Users [IN:3052]
    - Open Redirection via ReturnUrl Parameter [IN:3053]
    - HTTP Cacheable Response Changes [IN:3054]
    - Internal Path Disclosure in Error Messages [IN:3055]
    - SMTP Recipient Injection via User Registration Form [IN:3056]
    - Lack of Error Handling [IN:3057]
    - Emails sent out with new 'Note' added when no new note is added. [IN:3069]
    - Extra entries in tst_artifact_attachment table.. [IN:3072]
    - Hide email addresses for users unless logged in user is a support agent type of role. [IN:3086]
    - Security Vulnerability: XSS issue with the global search box [IN:3203]
    - KronoDesk description box toolbar scrolls up if you enter more than 12 lines of text. [IN:3210]
    - Deleting user - filter user lists. [IN:3230]
    - When accessed from forum post, user profile does not include help desk tickets [IN:3281]
    - Need to validate the ReturnURL parameter used on some of the Account pages [IN:3293]
    - Consider enabling Viewstate encryption and enableviewstatemac for better security [IN:3295]
    - Application error; stopped working if a bad sort gets in the user's profile [IN:3324]
    - Paging issue on KronoDesk [IN:3334]
    - We need to handle XSS injection in tickets that are initiated from email. [IN:3355]
    - Edit Admin -> Roles page for better clarity. [IN:3372]
    - Add 'guest' role.. [IN:3373]
    - Add code syntax highlighting to Knowledge Base [IN:3405]
    - Thread page timing of 0 should be '0 minutes' not '0 minute' [IN:3458]
    - Duplicate validation messages on new ticket creation [IN:3459]
    - RSS Token on Account Page [IN:3569]
    - [Vulnerability Report] Persistent XSS at Inflectra forums [IN:3643]
    - Knowledge Base - if all sub categories of a category have no articles, the sub category heading is still displayed (though the sub categories themselves are not) [IN:3648]
    - v2.0 Installer Issues [IN:3787]
    - When a new email message comes in for a deleted ticket, it's simply being added to the deleted ticket [IN:3797]
    - When an administrator is editing a user's profile, hide the "change password" button. [IN:3827]
    - Administrator editing a user's profile causes avatar to revert to original [IN:3828]
    - When you paste a screenshot in a new note and try to save, you get an error about it being changed by someone else. [IN:3831]
    - Ticket history dates are garbled: for example "23/10/17" for January 10, 2017. [IN:3832]
    - The Home Link on the Knowledge Base has the Wrong URL [IN:3833]
    - Cannot create a new user in admin or register for an account [IN:3834]
    - Link from individual KB article to the category does not work [IN:3836]
    - Ticket detail page: upon changing/selecting a product, hidden custom fields appear and asterisks disappear [IN:3838]
    - With Edge browser, the function to paste a screenshot does not work [IN:3839]
    - Some ticket list fields get filled in with the first value (automatically, not by the user) [IN:3840]
    - Ticket history problem: for newly-defined custom properties, the field name is strange [IN:3841]
    - saved draft articles cannot be accessed from user page [IN:3842]
    - Adding links and attachments to Articles does not work properly [IN:3843]
    - Article tag cloud should only show top 25 tags [IN:3844]
    - External home page, Recent Articles widget: time is off by 5 hours [IN:3847]
    - Get error when try to edit articles that have been created today (OK with the sample data) [IN:3851]
    - Knowledge Base main page: minor display issues if subcategories are defined but don't contain any articles [IN:3852]
    - KB: the first article in each subcategory is missing from the subcategory page [IN:3853]
    - Administration: Help Desk custom property editing problems [IN:3854]
    - Help Desk list page: text in error pop-up is incorrect [IN:3856]
    - Help Desk list page: need to fix the text that briefly appears while the list is loading [IN:3858]
    - User account page: trying to go to the second page of the "My Published KB Articles" section gives an error [IN:3859]
    - Administration Event Log: event detail pop-up does not scroll. [IN:3860]
    - Admin, System Settings, Product Definitions page: workflow dropdown shows "All selected" when only one workflow exists. [IN:3862]
    - Admin, Help Desk Settings, Workflows: Wrong message when attempting to delete an active workflow [IN:3863]
    - New ticket page: problems with attachments [IN:3864]
    - Help desk ticket list: Merge Tickets button on left side does not do anything [IN:3867]
    - Some custom property options are not working [IN:3868]
    - If you try and login using the Login.aspx page (not the popup) no messages are shown on failure [IN:3872]
    - Draft article can be viewed by anyone, whether logged in or not, with URL [IN:3874]
    - New ticket page no longer gives you a message at the top of the screen about missing required fields... [IN:3875]
    - Attachments to Knowledge Base articles cannot be viewed if not logged in [IN:3877]
    - Enable spell checking function wherever possible. [IN:3878]
    - Knowledge base: there is no way to remove attachments from articles [IN:3879]
    - Help Desk: function to delete attachment from ticket is not working. [IN:3880]
    - Internal Home page: under Draft KB Articles, the links are incorrect. [IN:3882]
    - Security: person logged in with default user role is able to view ticket attachments by using the URL [IN:3883]
    - When not logged in, attempting to view a forum thread gives an error [IN:3884]
    - User whose role does not have view permission for articles can still view articles [IN:3896]
    - External role with edit permission for forum messages is able to edit all replies. [IN:3898]
    - Most Event Notifications are not being triggered [IN:3901]
    - Admin System settings, E-Mail Configuration: changes to message templates are not saved [IN:3902]
    - Administration > Help Desk Settings > Event Notifications: email templates are not used [IN:3903]
    - Notifications are mixed up: adding a note sends email for different events [IN:3905]
    - Workflow: function to configure Ticket Note as required does not work [IN:3906]
    - Workflow: function to configure custom rich text property as hidden does not work [IN:3907]
    - Workflow: Required custom properties are not marked as such for internal users (external OK) [IN:3908]
    - Need to double-check Installer's Workflow 'Field Status' upgrade. [IN:3909]
    - Admin -> Error Log, 'Clear All' button doesn't seem to clear. [IN:3910]
    - Customer getting an error trying to save ticket [IN:3913]
    - For customer role, using betatest.kronodesk.net, the ticket detail page takes 30 seconds to load [IN:3919]
    - On the test site, betatest.kronodesk.net, the default role is User. It should be Customer, [IN:3920]
    - On the Account Verification Resend page, when you enter an unknown email address, no message comes up (updated) [IN:3924]
    - Installation issue: On a newly upgraded KronoDesk site, on user profiles, the Spira login & API key fields are hidden. [IN:3929]
    - Annoying to have to scroll up to change workflow status [IN:3930]
    - Administration -> Edit Profile page: no roles are displayed [IN:3940]
    - Ticket list: external user can see internal note in tooltip. [IN:3943]
    - Changing your own password isn't working. It's giving an error. [IN:3944]
    - Installer missing file in /images [IN:3952]