# Minimal Hybrid Configuration

 Smaller organizations that do not intend to have coexistence between an on-premises Exchange organization and Exchange Online for an extended time should consider running a minimal hybrid configuration, also known as an express migration. This hybrid migration option involves less complexity but also has less functionality than a full hybrid configuration.

A minimal hybrid configuration is similar to a full hybrid configuration in that they both allow you to migrate mailboxes incrementally; however, a minimal hybrid configuration lacks most of the integrated functionality that is contained in a full hybrid configuration. You should not use the minimal hybrid configuration option during a migration from an on-premises Exchange organization to Exchange Online, which will be relatively short because of the limited coexistence features.

A minimal hybrid configuration does not include.

 *  Federation.
 *  Secure email transfer.
 *  Free/busy lookups between on-premises and cloud.
 *  Redirection for Outlook on the web and ActiveSync clients

You can perform mailbox moves from an on-premises Exchange organization to Exchange Online by using the Exchange admin center, just as you would with a full hybrid configuration. In addition, Outlook clients are automatically reconfigured when mailboxes are moved. There is mail flow between the on-premises Exchange organization and Exchange Online; however, the messages are not guaranteed to be secured by TLS. Messages are secured by TLS if opportunistic TLS is successful.

When you select the **Minimal Hybrid Configuration** option in the Hybrid Configuration wizard, and if you have not configured Azure AD Connect for directory synchronization, the Hybrid Configuration wizard provides an option to perform a one-time directory sync of users and passwords. The wizard provides the steps to download and install Azure AD Connect for a one-time sync. Alternatively, you can install it later on your own.

‎