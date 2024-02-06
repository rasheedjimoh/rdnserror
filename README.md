# Fixing RDP error rdns error
## Error

realm: Couldn't join realm: Insufficient permissions to join the domain

![insufficient permission](https://github.com/rasheedjimoh/rdnserror/assets/157264080/167b8773-c6ac-4f07-b661-57f8c79809c1)


## Resolution
When setting up your computer to join a domain, you might encounter a situation where the Reverse DNS (rdns) is set to false. It's a bit like your computer trying to speak a specific language to enter a club, but it's also checking names in reverse, which is unnecessary.

To fix this, you need to dive into the computer's configuration files, specifically the /etc/krb5.conf file. Within this file, you'll find a setting for rdns, and you have to change it to false. It's essentially telling your computer, "Hey, don't bother checking names in reverse anymore!"

After making this adjustment, you'll need to restart your computer for the changes to take effect. This tweak ensures that your computer can smoothly join the domain without unnecessary checks that might have been causing issues.

![resolution](https://github.com/rasheedjimoh/rdnserror/assets/157264080/75a29856-a542-441d-96bd-db7fe13ad71c)
