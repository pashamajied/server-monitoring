# server-monitoring
Shell Script to Monitoring server from your VPS (AWS, Alibaba Cloud, Digital Ocean, Vultr).
Be sure to edit the configuration options at the beginning of the script to match your environment prior to executing.

# Usage:

1. Pull up a terminal or SSH into the target server.

2. Logon as root

<pre>sudo -i</pre>

3. Download the script(s).

<pre>wget https://raw.githubusercontent.com/pashamajied/server-monitoring/master/server-monitoring.sh</pre>

4. Edit the configuration options at the beginning of the script to match your environment prior to executing.
<pre>
#telegram conf
GROUP_ID=xxxxxxxxx
BOT_TOKEN=xxxxxxxxxx:xxxxxxxxxxxx-xxxxxxx-xxxxxxxxxxxxxx
</pre>

5. Make the script executable

<pre>chmod +x server-monitoring.sh</pre>

6. Run the script.

<pre>./server-monitoring.sh</pre>

8. Setup a cronjob to run the script daily/weekly if you choose.
<pre>
0 6   * * * /opt/server-monitoring.sh >/dev/null 2>&1
</pre>
