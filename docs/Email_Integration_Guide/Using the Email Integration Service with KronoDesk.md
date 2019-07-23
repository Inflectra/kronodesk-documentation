# Using the Email Integration Service with KronoDesk

Once you have the email integration service configured, we recommend
that you initially clear the Windows Application Log on the machine.
This will allow you to quickly see any errors that occur due to
misconfiguration. The event viewer can be found in Control Panel \>
Administrative Tools \> Event Viewer.

Once you have the email integration enabled and running, any users that
email in a support ticket to one of the "watched" email addresses will
experience the following process:

1.  The customer emails <support@mycompany.com> with a help desk
request.

2.  The contents (including attachments) of the email will be parsed by
the email integration service and a new help desk ticket will be
created in KronoDesk.

3.  The customer will receive an automated email from the system letting
them know that the ticket was received:


> \-\-\-\-\--=\> Please keep your reply above this line. \<=-
> 
> Hello Fred Bloggs
> 
> The following ticket in My Company support system has been recently
> updated:
> 
> Name: \#TK438 - test 123
> 
> Priority:
> 
> Status: Open
> 
> Product: Product 1
> 
> Type:
> 
> Assignee:
> 
> Last Updated: 10/19/2012 4:29:37 PM
> 
> To view the ticket, click the URL below:
> 
> <http://mycompany.kronodesk.net/Ticket/438.aspx>

4.  If this is the first time the user has ever submitted a help desk
ticket, the system will also create a new **unverified** user
account in KronoDesk on behalf of this user.

-   The user will then receive a separate email with information
about their new account. It will provide a hyperlink that allows
them to "verify" this new user account so that they can
view/modify their help desk tickets through the website.

-   If the user clicks on this verify link, they will be taken to
KronoDesk, where they will have the option of providing a
password and other security information that will allow them to
access the support system through the website. If they don't
verify the account, they can still respond to the ticket through
email.

5.  The customer service manager(s) will assign the ticket to the
appropriate customer service agent and the assigned agent will add
information to the ticket either providing a possible solution to
the enquiry or requesting additional information.

-   In either case, the customer will receive an email containing
the note(s) from the customer service agent.

6.  The customer can either verify their account and reply to the agent
through the KronoDesk web interface, or they can simply reply to the
email notifications, making sure that their comments are **above the
special line marked "please reply above this line"**. Any text that
is entered above this line will be added to the help desk ticket as
a new note. Any attachments will be added to the existing
attachments linked to the ticket

7.  This process continues until the customer's enquiry is resolved.

