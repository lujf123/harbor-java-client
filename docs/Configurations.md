# Configurations

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authMode** | **String** | The auth mode of current system, such as \&quot;db_auth\&quot;, \&quot;ldap_auth\&quot; |  [optional]
**emailFrom** | **String** | The sender name for Email notification. |  [optional]
**emailHost** | **String** | The hostname of SMTP server that sends Email notification. |  [optional]
**emailPort** | **Integer** | The port of SMTP server. |  [optional]
**emailIdentity** | **String** | By default it&#x27;s empty so the email_username is picked. |  [optional]
**emailUsername** | **String** | The username for authenticate against SMTP server. |  [optional]
**emailSsl** | **Boolean** | When it&#x27;s set to true the system will access Email server via TLS by default.  If it&#x27;s set to false, it still will handle \&quot;STARTTLS\&quot; from server side. |  [optional]
**emailInsecure** | **Boolean** | Whether or not the certificate will be verified when Harbor tries to access the email server. |  [optional]
**ldapUrl** | **String** | The URL of LDAP server. |  [optional]
**ldapBaseDn** | **String** | The Base DN for LDAP binding. |  [optional]
**ldapFilter** | **String** | The filter for LDAP binding. |  [optional]
**ldapScope** | **Integer** | 0-LDAP_SCOPE_BASE, 1-LDAP_SCOPE_ONELEVEL, 2-LDAP_SCOPE_SUBTREE |  [optional]
**ldapUid** | **String** | The attribute which is used as identity for the LDAP binding, such as \&quot;CN\&quot; or \&quot;SAMAccountname\&quot; |  [optional]
**ldapSearchDn** | **String** | The DN of the user to do the search. |  [optional]
**ldapTimeout** | **Integer** | timeout in seconds for connection to LDAP server. |  [optional]
**ldapGroupAttributeName** | **String** | The attribute which is used as identity of the LDAP group, default is cn. |  [optional]
**ldapGroupBaseDn** | **String** | The base DN to search LDAP group. |  [optional]
**ldapGroupSearchFilter** | **String** | The filter to search the ldap group. |  [optional]
**ldapGroupSearchScope** | **Integer** | The scope to search ldap. &#x27;0-LDAP_SCOPE_BASE, 1-LDAP_SCOPE_ONELEVEL, 2-LDAP_SCOPE_SUBTREE&#x27; |  [optional]
**ldapGroupAdminDn** | **String** | Specify the ldap group which have the same privilege with Harbor admin. |  [optional]
**projectCreationRestriction** | **String** | This attribute restricts what users have the permission to create project.  It can be \&quot;everyone\&quot; or \&quot;adminonly\&quot;. |  [optional]
**readOnly** | **Boolean** | &#x27;docker push&#x27; is prohibited by Harbor if you set it to true.    |  [optional]
**selfRegistration** | **Boolean** | Whether the Harbor instance supports self-registration.  If it&#x27;s set to false, admin need to add user to the instance. |  [optional]
**tokenExpiration** | **Integer** | The expiration time of the token for internal Registry, in minutes. |  [optional]
**verifyRemoteCert** | **Boolean** | Whether or not the certificate will be verified when Harbor tries to access a remote Harbor instance for replication. |  [optional]
**scanAllPolicy** | **Object** |  |  [optional]
