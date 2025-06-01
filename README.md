# Cybersecurity internship task-4
1. Open Firewall Configuration Tool:

    Press Win + R, type wf.msc, and press Enter.

        This opens Windows Defender Firewall with Advanced Security.

2. List Current Firewall Rules:

    Navigate to:

        Inbound Rules (left pane) → see all existing inbound rules.

        Outbound Rules → for outbound traffic.

3. Add a Rule to Block Port 23 (Telnet):

    In left pane → Click Inbound Rules → then right-click → New Rule...

        Choose Port → TCP → enter 23 → click Next.

        Choose Block the connection → Next.

        Apply to Domain, Private, Public → Next.

        Name it something like "Block Telnet Port 23" → Finish.

4. Test the Rule:

    Use telnet from another system or command prompt (if installed):

    telnet <ip_address> 23

        Should fail to connect if rule is active.

5. SSH Not Required on Windows, skip.
6. Remove the Test Rule:

    Go back to Inbound Rules.

    Find "Block Telnet Port 23", right-click → Delete.

7. Documentation of GUI Steps:

    Access via wf.msc.

    Inbound Rules → New Rule → Port 23 → Block → Apply.

    Later, delete rule via right-click
