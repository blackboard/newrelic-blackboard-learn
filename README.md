This repo contains the New Relic instrumentation for Blackboard Learn that could not be implemented with Java API and annotations.

To install New Relic Java application agent in Blackboard Learn v.201404 and above, follow these instructions:

1. Download New Relic Java application agent archive and extract the "newrelic" folder into the 'apps' directory
2. Modify 'bb-config.properties' file to include '-javaagent:/usr/local/blackboard/apps/newrelic/newrelic.jar' in 'bbconfig.jvm.options.extra.tomcat'
3. Apply the extensions instrumentation in this repo
4. Run PushConfigUpdates for the bb-config change to take effect and the Tomcat container to restart
