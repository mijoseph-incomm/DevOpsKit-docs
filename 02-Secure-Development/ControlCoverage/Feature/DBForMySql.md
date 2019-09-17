<html>
<head>

</head><body>
<H2>DBForMySQL</H2><table><tr><th>Description & Rationale</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td><b>Use the 'Allow access to Azure services' flag or IP range only if required</b><br/>The 'Allow access to Azure services' setting configures a very broad range of IP addresses from Azure as permitted to access the MySQL Server. Please make sure your scenario really requires this setting before enabling it. Turning it ON exposes your MySQL Server to risk of attacks from resources (IPs) owned by others in the Azure region.</td><td>High</td><td>Yes</td></tr><tr><td><b>Configure only the required IP addresses on MySQL server. Do not use 'Any-to-Any' IP range.</b><br/>Using the firewall feature ensures that access to the data or the service is restricted to a specific set/group of clients. NOTE: While this control does provide an extra layer of access control protection, it may not always be feasible to implement in all scenarios.</td><td>High</td><td>Yes</td></tr><tr><td><b>SSL connection must be enabled for Azure Database for MySQL</b><br/>Enforcing SSL connections between your database server and your client applications helps protect against 'man in the middle' attacks by encrypting the data stream between the server and your application.</td><td>High</td><td>Yes</td></tr><tr><td><b>Consider using virtual network rules for improved isolation</b><br/>Virtual network rules provides isolation for your Azure Database for MySQL by permitting only the specified virtual networks to access the database server.</td><td>Medium</td><td>Yes</td></tr><tr><td><b>Backup and Disaster Recovery must be planned at the time of creation of Azure Database for MySql service</b><br/>Azure Database for MySQL offers default backup/disaster recovery for 7 days that can be extended up to 35 days. You can choose between locally redundant or geo-redundant backup storage. When processing critical workloads, a team must have adequate backups of the data.</td><td>Medium</td><td>Yes</td></tr><tr><td><b>Advanced Threat Protection must be enabled for Azure Database for MySQL</b><br/>Advanced Threat Protection for Azure Database for MySQL provides a layer of security, which enables customers to detect and respond to potential threats as they occur by providing security alerts on anomalous activities.</td><td>High</td><td>Yes</td></tr><tr><td><b>Diagnostics logs must be enabled with a retention period of at least365 days.</b><br/>Logs should be retained for a long enough period so that activity trail can be recreated when investigations are required in the event of an incident or a compromise. A period of 1 year is typical for several compliance requirements as well.</td><td>Medium</td><td>Yes</td></tr><tr><td><b>Diagnostic and activity logs for Azure Database for MySQL should be reviewed periodically</b><br/>Periodic reviews of diagnostics, activity and audit logs ensures that anomalous activity can be identified early enough instead of after a major compromise.</td><td>Medium</td><td>No</td></tr><tr><td><b>Access to Azure Database for MySQL Servers must be granted in accordance with the principle of least privilege</b><br/>Granting minimum access ensures that users are granted just enough permissions to perform their tasks. This minimizes exposure of the resources in case of user/service account compromise.</td><td>High</td><td>No</td></tr><tr></table>
<table>
</table>
</body></html>