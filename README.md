check_smb_share
===============

Nagios plugin to check SMB share accessibility 

Uses smbclient to produce a share list and check if shares are there. Will drop back to an 
anonymous login if you haven't disabled them (bad!). Otherwise, effectively verifies that
the user account can login and samba is basically functioning.

Usage:
  check_smb_share -H <host> -s <sharename>
  check_smb_share -H <host> -s <sharename> -u <user> -p <password> -d <domain>

