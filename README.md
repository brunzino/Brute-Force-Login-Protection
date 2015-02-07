# Brute Force Login Protection
Protects your WordPress website against brute force login attacks using .htaccess

## Description
A Brute Force Attack aims at being the simplest kind of method to gain access to a site: it tries usernames and passwords, over and over again, until it gets in.
Brute Force Login Protection is a lightweight plugin that protects your website against brute force login attacks using .htaccess.

After a specified limit of login attempts within a specified time, the IP address of the hacker will be blocked.

### Features

* Limit the number of allowed login attempts using normal login form
* Limit the number of allowed login attempts using Auth Cookies
* Manually block/unblock IP addresses
* Manually whitelist trusted IP addresses
* Delay execution after a failed login attempt (to slow down brute force attack)
* Option to inform user about remaining attempts on login page
* Option to email administrator when an IP has been blocked
* Custom message to show to blocked users

Your feedback is highly appreciated!

## Installation
1. Install the plugin either via the WordPress.org plugin directory, or by uploading the files to your wp-content/plugin directory.
2. Activate the plugin through the WordPress admin panel.
3. Customize the settings on the settings page.
4. Done!

## Frequently Asked Questions
### My own IP is blocked, what do I do?
If you have FTP access to your website edit the .htaccess file and remove the line: 'deny from x.x.x.x', where x.x.x.x is your own IP address.
If you don't have FTP access, the only way to unblock your IP is to log in your WordPress admin panel from another IP address and unblock it via the plugin settings page.

### I get an error: .htaccess file not readable/writeable
Brute Force Login Protection will only work if your .htaccess file is writeable by WordPress. If you get this error, make sure that your .htaccess file has read and write permissions.

## Changelog
### 1.4.1
* Option to email administrator when an IP has been blocked
* Button to whitelist your current IP
* Bugfixes and improvements

### 1.4
* Ability to whitelist trusted IPs
* Ability to create custom message to show to blocked users
* Delay execution after a failed login attempt (to slow down brute force attack)
* Performance improvements

### 1.3
* Protection against brute force attacks using Auth Cookies

### 1.2
* Option to inform user about remaining attempts on login page
* Ability to reset options
* Status panel on the settings page

### 1.1
* Added Dutch translation

### 1.0
* Initial version