.. This work is licensed under a Creative Commons Attribution 4.0 International License.

Log Enhancements Release Notes
==============================

Version: 3.0.1 Casablanca Release
--------------
Casablanca
--------------
   - logging-analytics Version: 1.2.6

--------------
:Release Date: 2019-02-08

**New Features**
   - kubernetes installation upped to 1.11.5 in the Rancher 1.6.25 RI
   - NFS support for AWS EFS

**Bug Fixes**
   - `LOG-837 <https://jira.onap.org/browse/LOG-837>`_ Logging/POMBA CLM: fix/address/red-flag spring-mvc-5.1.2 pulls in spring-web-5.0.9

**Known Issues**

   - `LOG-376 <https://jira.onap.org/browse/LOG-376>`_ Logstash load balancing is asymmetric wherever AAI is run
   - `LOG-895 <https://jira.onap.org/browse/LOG-895>`_ Upgrade Rancher to 1.6.25 to address CVE-2018-1002105 and move to Kubernetes 1.11.5 (server side)

**Security Notes**

LOG code has been formally scanned during build time using NexusIQ and all Critical vulnerabilities have been addressed, items that remain open have been assessed for risk and determined to be false positive. The LOG open Critical security vulnerabilities and their risk assessment have been documented as part of the `project <https://wiki.onap.org/pages/viewpage.action?pageId=45307852>`_.

Quick Links:
 	- `LOG project page <https://wiki.onap.org/display/DW/Logging+Enhancements+Project>`_

 	- `Passing Badge information for LOG <https://bestpractices.coreinfrastructure.org/en/projects/1578>`_

 	- `Project Vulnerability Review Table for LOG <https://wiki.onap.org/pages/viewpage.action?pageId=45307852>`_

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      None


POMBA Release Notes
--------------
POMBA is sub-project of the Logging Enhancements Project.

Casablanca
--------------
   - pomba-audit-common Version: 1.3.2
   - pomba-aai-context-builder Version: 1.3.2
   - pomba-context-aggregator Version: 1.3.4
   - pomba-network-discovery-context-builder Version: 1.3.1
   - pomba-sdc-context-builder Version: 1.3.2

--------------
:Release Date:  2019-02-08

**New Features**
   - Version 1 of the audit common model
   - Initial release of context aggregator and 3 context builders

**Bug Fixes**

   - `LOG-892 <https://jira.onap.org/browse/LOG-892`_ PORT - POMBA Network Discovery Context Builder does not log

**Known Issues**

   - `LOG-913 <https://jira.onap.org/browse/LOG-913>`_ POMBA: 1 of 11 pods failing on sequenced startup on 3.0.0-ONAP - pomba is 22 on the order - looks timing related
   - `LOG-950 <https://jira.onap.org/browse/LOG-950>`_ LOG-950 upped the numbers from 10 to 30 – for intermittent deploy timing – this is an issue for several projects since 3.0.0-ONAP - the solution is a sequenced 5h deploy via `cd.sh <https://git.onap.org/logging-analytics/tree/deploy/cd.sh#n228>`_ and/or better vms for now until the `dependencies <https://wiki.onap.org/display/DW/Log+Streaming+Compliance+and+API#LogStreamingComplianceandAPI-DeploymentDependencyTree-Containerlevel>`_ and jobs are refactored into helm hooks

**Security Notes**
   - all three nodeports for kibana, context builder and data-router are open by default for now

POMBA code has been formally scanned during build time using NexusIQ and all Critical vulnerabilities have been addressed, items that remain open have been assessed for risk and determined to be false positive. The LOG open Critical security vulnerabilities and their risk assessment have been documented as part of the `project <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_.

Quick Links:
   - `POMBA project page <https://wiki.onap.org/display/DW/POMBA>`_
   - `See the result from LOG <https://bestpractices.coreinfrastructure.org/en/projects/1578>`_
   - `See the result from LOG <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      None


Version: 1.2.2 Casablanca
--------------

:Release Date: 2018-11-30

**New Features**
   - Demo slf4j library with marker/mdc support along with kubernetes, docker, war support projects.

**Bug Fixes**


**Known Issues**
   - `Logstash load balancing is asymmetric wherever AAI is run <https://jira.onap.org/browse/LOG-376>`_

**Security Notes**

LOG code has been formally scanned during build time using NexusIQ and all Critical vulnerabilities have been addressed, items that remain open have been assessed for risk and determined to be false positive. The LOG open Critical security vulnerabilities and their risk assessment have been documented as part of the `project <https://wiki.onap.org/pages/viewpage.action?pageId=45307852>`_.

Quick Links:
 	- `LOG project page <https://wiki.onap.org/display/DW/Logging+Enhancements+Project>`_

 	- `Passing Badge information for LOG <https://bestpractices.coreinfrastructure.org/en/projects/1578>`_

 	- `Project Vulnerability Review Table for LOG <https://wiki.onap.org/pages/viewpage.action?pageId=45307852>`_

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      None


POMBA Release Notes
--------------
POMBA is sub-project of the Logging Enhancements Project.

Casablanca
--------------
   - pomba-audit-common Version: 1.3.1
   - pomba-aai-context-builder Version: 1.3.1
   - pomba-context-aggregator Version: 1.3.3
   - pomba-network-discovery-context-builder Version: 1.3.0
   - pomba-sdc-context-builder Version: 1.3.1


--------------

:Release Date: 2018-11-15

**New Features**
   - Version 1 of the audit common model
   - Initial release of context aggregator and 3 context builders

**Bug Fixes**


**Known Issues**


**Security Notes**
   - all three nodeports for kibana, context builder and data-router are open by default for now

POMBA code has been formally scanned during build time using NexusIQ and all Critical vulnerabilities have been addressed, items that remain open have been assessed for risk and determined to be false positive. The LOG open Critical security vulnerabilities and their risk assessment have been documented as part of the `project <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_.

Quick Links:
   - `POMBA project page <https://wiki.onap.org/display/DW/POMBA>`_
   - `See the result from LOG <https://bestpractices.coreinfrastructure.org/en/projects/1578>`_
   - `See the result from LOG <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      None

Version: Beijing
--------------

:Release Date: 2018-06-07

**New Features**
   - Logstash is a daemonset (clustered at 1 container per VM)
   - `The following applications send logs to the ELK stack - <https://jira.onap.org/browse/LOG-230>`_

**Bug Fixes**


**Known Issues**
   - Logstash load balancing is asymmetric

**Security Notes**
   - all three nodeports for logstash, elasticsearch and kibana are open by default for now

LOG code has been formally scanned during build time using NexusIQ and all Critical vulnerabilities have been addressed, items that remain open have been assessed for risk and determined to be false positive. The LOG open Critical security vulnerabilities and their risk assessment have been documented as part of the `project <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_.

Quick Links:
 	- `LOG project page <https://wiki.onap.org/display/DW/Logging+Enhancements+Project>`_

 	- `Passing Badge information for LOG <https://bestpractices.coreinfrastructure.org/en/projects/1578>`_

 	- `Project Vulnerability Review Table for LOG <https://wiki.onap.org/pages/viewpage.action?pageId=28378692>`_

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      Note: there was no released artifacts under 1.2.2 for Beijing - release was pushed to Casablanca



Version: 1.0.0
--------------

:Release Date: 2017-11-16

**New Features**

This release adds Elastic Stack analytics deployment to OOM, aligns logging provider configurations, and fixes issues with the propagation of transaction IDs and other contextual information.

    - `LOG-1 <https://jira.onap.org/browse/LOG-1>`_ Transaction ID propagation.
    - `LOG-2 <https://jira.onap.org/browse/LOG-2>`_ Standardized logging provider configuration.
    - `LOG-3 <https://jira.onap.org/browse/LOG-3>`_ Elastic Stack reference analytics pipeline.
    - `LOG-4 <https://jira.onap.org/browse/LOG-4>`_ Transaction ID conventions.

**Bug Fixes**

    - `LOG-64 <https://jira.onap.org/browse/LOG-64>`_ Logger field has a length restriction of 36 which needs a fix.
    - `LOG-74 <https://jira.onap.org/browse/LOG-74>`_ Extract componentName from the source path of log files.

**Known Issues**

    - `LOG-43 <https://jira.onap.org/browse/LOG-43>`_
      Unable to find logback xml for DMaaP component.
      Logging file for DMaaP is available in this jar "eelf-core-0.0.1.jar".

    - `LOG-65 <https://jira.onap.org/browse/LOG-65>`_
      SO Logging Provider Config File need correction in Timestamp MDC.
      Logging provider configuration file for SO i.e. logback files requires correction in Timestamp MDC for correct MDC generation in log.
      The current pattern prints Timestamp as 2017-09-25 05:30:07,832. Expected  pattern is - 2017-09-25T05:30:07.832Z.

    - `LOG-80 <https://jira.onap.org/browse/LOG-80>`_ Kibana does not seem to show all the logs from application pods.
      The content of the log directories (/var/log/onap/mso) are not 100% reflected in Kibana.

    - `LOG-88 <https://jira.onap.org/browse/LOG-88>`_
      SO log format error during Health Check - blocking tracking jira for SO-246.

**Security Issues**
      None

**Upgrade Notes**
      None

**Deprecation Notes**
      None

**Other**
      None

===========

End of Release Notes
