This repo contains the New Relic instrumentation for Blackboard Learn that could not be implemented with Java API and annotations.

To install New Relic Java application agent in Blackboard Learn v.201404 and above, follow these instructions:

1. Download New Relic Java application agent archive and extract the 'newrelic' folder into the 'apps' directory
2. Verify your 'license_key' in 'newrelic.yml' file
2. Modify 'bb-config.properties' file to include '-javaagent:/usr/local/blackboard/apps/tomcat/newrelic/newrelic.jar' on 'bbconfig.jvm.options.extra.tomcat'
3. Copy the "extensions" folder from this repo into the "newrelic" folder and change the owner of the directory to bbuser
4. Run PushConfigUpdates for the configuration change to take effect

For viewing JMX metrics, refer to New Relic's instructions:
https://docs.newrelic.com/docs/agents/java-agent/custom-instrumentation/custom-jmx-instrumentation-yaml#display_metrics
