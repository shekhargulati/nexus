Nexus on OpenShift
============================

This git repository will help you get up and running quickly with nexus running on tomcat on OpenShift.

Create a DIY app on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ , don't forget to create a namespace and install client tools as well.

Create a DIY application

    rhc app create -a nexus -t diy-0.1

Get Nexus running
----------------------------
Grab this quickstart codes and make it working for you!

    cd nexus
    git remote add nexus git@github.com:shekhargulati/nexus.git
    git pull -s recursive -X theirs nexus master

Next download the war from Sonatype website http://www.sonatype.org/downloads/nexus-2.1.2.war and copy into diy/tomcat/webapps directory and rename it to nexus.war

Finally do git push and see nexus running on OpenShift.
That's it, you can now checkout your nexus at:

    http://nexus-$yournamespace.rhcloud.com/nexus

The default nexus user is admin/admin123
