# APEX Sending Emails

Some of the points you need to know about sending emails from APEX on OCI are you can use the **APEX_MAIL** PL/SQL API to send emails from Oracle APEX. 

But before you use APEX mail or any other mailing features of Oracle APEX, you must configure an email provider in your APEX instance. Currently, the only supported email provider is the **OCI Email Delivery Service**.

## Configuration Steps

1. Generate SMTP Credetentials for Email Delivery
2. Create an approved sender for Email Delivery
3. Configure the STMP Parameters in the APEX instance
4. Send a test email using APEX Workshop

When you submit a mail using the APEX_MAIL PL/SQL or any other mailing services available within APEX, the mails are not sent immediately. The mails are first added to a **mail queue**, which are then processed by a separate database job which runs every five minutes.

As an instance administrator, you can manage emails sent from applications by monitoring email messages in the mail queue and mail log by logging into the APEX Administration Services. Using the mail queue, you can push, delete, or reset messages that have to be sent.

## Understanding APEX_MAIL

APEX_MAIL package is a wrapper around the Oracle-supplied UTL_SMTP package. 

Notable procedures:

- SEND
- PUSH_QUEUE
- ADD_ATTACHMENT

APEX installs the database job, and the name of the job is ORACLE_APEX_MAIL_QUEUE. This job periodically sends all the mails stored in the active mail queue.

## On-Prem Database or Non-Autonomous Database

If you are hosting APEX instance on an on-prem database or on a non-Autonomous Database, you will have to enable network services to send outbound mails in Oracle APEX. By default, the network services are disabled, and you would have to enable these services manually. You can do that by using the DBMS_NETWORK_ACL_ADMIN package to grant necessary connect privileges to any email host for the APEX Database user.
