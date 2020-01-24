# Step 1: Create a DNS zone in Lightsail

- If you don't have an AWS account yet, create one here: https://aws.amazon.com/. Once created, log in to your AWS account and navigate to https://lightsail.aws.amazon.com/. 

- Click "Create DNS zone" under the "Networking" tab
![New DNS Zone in Lightsail](/images/create_dns_zone.png)

- Enter your domain name including the TLD and click "Create DNS Zone" 
![Create DNS Zone](/images/create_dns_zone_2.png)

- Once created, your DNS Zone will display a list of Name servers
![Name servers](/images/nameservers.png)

Copy these down, we'll need them in the next step.

# Step 2: Edit the name servers list in Domain.com

- Log in to domain.com and click on "Manage" for your domain
![Manage your domain](/images/domain_com_manage.png)

- On the left panel, click "DNS & Nameservers"

![DNS & Nameservers](/images/domain_com_nameservers.png)

- Click "Add Nameserver" and add the four name server URLs from Step 1
![Add Nameservers](/images/domain_com_add_ns.png)

- Delete the old nameservers
![Delete old nameservers](/images/domain_com_remove_ns.png)

- Your final result should look like this (your name server URLs will be different)
![Final Reference](/images/domain_com_final.png)

# Step 3: Add DNS Records in Lightsail

- Open the lightsail console (https://lightsail.aws.amazon.com/), click the "Networking" tab and click on your DNS Zone. You can now manage DNS records directly from Lightsail. 
![Lightsail DNS](/images/ls_add_records.png)

This is a handy way to manage your virtual machines, static IP addresses, and DNS records all in one place. 
