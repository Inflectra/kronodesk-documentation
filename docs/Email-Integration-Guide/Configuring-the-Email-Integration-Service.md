# Configuring the Email Integration Service

Once you have completed the installation, you can configure the email
integration service by going to Start \> Program Files \> Inflectra
SpiraTeam \> Tools \> Email Integration which will bring up the
management interface.

![](img/Configuring_the_Email_Integration_Service_6.png)




## Connecting to the KronoDesk Server

The first tab lets you specify the KronoDesk instances that the email
integration service will connect to. To add a new KronoDesk server,
click on the green Add (+) icon to switch the screen to allow you to
enter a new KronoDesk server:

![](img/Configuring_the_Email_Integration_Service_7.png)




You need to enter the following information:

-   **Server URL -** The URL to KronoDesk server

-   **Account Login -** The account login that will be used to connect
to KronoDesk. It needs to be a user with the "administrator" role.

-   **Account Password -** This is the password for the account

Click the "Test" button to verify the connection. Once it has passed,
click the Save icon to save the new KronoDesk server information.

To modify an existing KronoDesk server instance, just click on its name
in the server list. To delete a server, select its name in the server
list and click the Delete icon (X).

Once you have entered all the KronoDesk instances that you will be
connecting to, click the "Next" button to move to the next tab and
configure the mail server integration.

## Connecting to the POP3 Mail Server

The "POP3 Accounts" tab displays a list of all the configured mail
servers:

![](img/Configuring_the_Email_Integration_Service_8.png)




Initially it will be empty, so just click the Add (+) icon to add a new
mail server:

![](img/Configuring_the_Email_Integration_Service_9.png)




You need to enter the following information:

-   **Account Email --** This should be the email address that will be
polled for new support emails.

-   **Mail Server --** This should be the fully-qualified name or IP
address of your POP3 mail server.

-   **Port --** This is the port that your mail server expects incoming
POP3 requests to use. The default for unencrypted POP3 requests is
110 and the default for SSL encrypted POP3 requests is 995.

-   **Use SSL --** You should check this option if your mail server
requires a secure SSL connection.

-   **Login/Password --** You should enter the login/password for the
mail server that allows reading of inbound messages for the email
address specified above.

-   **Remove Messages --** Checking this option will make the email
integration service remove the email messages from in the Inbox of
the user's email account. We recommend leaving this unchecked when
first using the service. Once you are happy that the integration is
correctly handling spam and not ignoring correct messages, you can
check this option to prevent the email inbox getting too large.

-   **Attach Message --** Checking this option will attach the original
email message to the new help desk ticket created in KronoDesk as
well as populating the ticket with the contents of the message. This
is useful when debugging a new installation but typically would be
unchecked during normal operation.

-   **Application Server --** You should specify the instance of
KronoDesk that this email account will be linked to.

-   **Default Product** -- KronoDesk requires that all new help desk
tickets be submitted with a selected product. If the inbound emails
have a product name specified in one of the email headers it will be
automatically routed to the correct product. In other cases, the
system will route the new help desk ticket to the default product
chosen in this setting.

-   **RegEx Match Content** -- Checking this option will allow the email
integration service to do a name match in the body of the email for
possible product names instead of just relying on the "default
product". For example if your email contains "Product1" in the
message text it will be routed to Product1 in KronoDesk.

## Configuring the Advanced Settings

Once you have finished configuring the KronoDesk server instances and
POP3 mail accounts, you can click on the "Advanced Settings" tab to
setup special rules that prevent emails from specific accounts being
processed as well as allow the email integration service to look for
special mail headers and subject tokens that might indicate bulk / spam
messages that should be ignored.

![](img/Configuring_the_Email_Integration_Service_10.png)




You can configure the following settings:

-   **Enable Trace Logging --** When this option is checked, the email
integration service will log information messages to the Windows
Application Event Log on the machine running the integration
service. This is useful when first deploying the system or when you
are encountering issues and Inflectra support personnel have asked
you switch on trace logging to aid in support. For normal use we
recommend turning this setting off to avoid too many messages being
logged in the Event Log.

-   **Minutes Between Polls --** This setting specifies the interval (in
minutes) between each time the email integration service attempts to
retrieve new email messages from the email server.

-   **Ignore Addresses --** In this section you can add a list of any
email addresses that you want to ignore and not use for creating new
KronoDesk help desk tickets. If there are any known senders or
internal email accounts, you should add them in this section.

In addition, there are two other sub-tabs to the Advanced Settings tab
that provide configuration options:

![](img/Configuring_the_Email_Integration_Service_11.png)




The "Ignore Headers" section allows you to specify any email message
headers that if present in an email message will be ignored by the email
integration service.

![](img/Configuring_the_Email_Integration_Service_12.png)




The "Ignore Keywords" section allows you to specify any keywords that if
present in the subject-line or body of an email message will be ignored
by the email integration service. Some mail servers that have built-in
SPAM detection systems will automatically add SPAM-HIGH, SPAM-MEDIUM,
SPAM-LOW to the subject line (for example).

