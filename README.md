## OPNsense Web Filter plugin
SquidGuard based plugin. 

**This plugin is non-official and EXPERIMENTAL use at your own risk.**


### Features:
- User based rules;
- Block websites based on categories;
- Custom block pages;
- RegEx based rules;

### Install and usage:

Logged as root run:
#`curl https://community.cloudfence.com.br/webfilter/setup.sh -o /tmp/setup.sh ; sh /tmp/setup.sh`

After installed, you will need to download a squidGuard compatible blacklist:

Ex.: https://docs.opnsense.org/manual/how-tos/proxywebfilter.html (Step 2 / UT1 category based list)

1-On the WebUI go to: **Services: Web Filter: General**

2-Set it in the `Blacklist Categories URL`

3-Click in the Download Button: The download and build database process can take several minutes (depending on the hardware)

4-Enable Web Filter & click Apply

5-Managing rules: https://wiki.cloudfence.com.br/english/managing-rules



### TODO
-Port the log viewer to the new OPNsense MVC standard

-Reset blacklist (remove and install it again)

-Multiple blacklists (maybe performance issues with - a lot testing needed!)

-Add groups support in rules; (port from Cloudfence plugin)

-Better frontend integration with Squid native  (a.k.a WebProxy)

-Add custom rules to squid (bandwith controls, mime-types based rules, etc)

-Improve Frontend features and capabilities; (with community help!)

-Improve Documentation

-Beautify the code ;-)  (I'm not a frontend guy, so please, be kind!)



