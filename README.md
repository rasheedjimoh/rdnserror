# Fixing RDP error rdns error

## Resolution
When setting up your computer to join a domain, you might encounter a situation where the Reverse DNS (rdns) is set to false. It's a bit like your computer trying to speak a specific language to enter a club, but it's also checking names in reverse, which is unnecessary.

To fix this, you need to dive into the computer's configuration files, specifically the /etc/krb5.conf file. Within this file, you'll find a setting for rdns, and you have to change it to false. It's essentially telling your computer, "Hey, don't bother checking names in reverse anymore!"

After making this adjustment, you'll need to restart your computer for the changes to take effect. This tweak ensures that your computer can smoothly join the domain without unnecessary checks that might have been causing issues.

