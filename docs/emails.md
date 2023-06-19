# APEX Sending Emails

Some of the points you need to know about sending emails from APEX on OCI are you can use the **APEX_MAIL** PL/SQL API to send emails from Oracle APEX. 

But before you use APEX mail or any other mailing features of Oracle APEX, you must configure an email provider in your APEX instance. Currently, the only supported email provider is the **OCI Email Delivery Service**.

## Configuration Steps

1. Generate SMTP Credetentials for Email Delivery
2. Create an approved sender for Email Delivery
3. Configure the STMP Parameters in the APEX instance
4. Send a test email using APEX Workshop