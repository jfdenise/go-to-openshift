FROM quay.io/jdenise/pipeline-wildfly-server:01c8773673fac13a3a53a7a9193e7008
COPY --chown=jboss:root deployments/* $JBOSS_HOME/standalone/deployments
COPY --chown=jboss:root extensions $JBOSS_HOME/extensions
RUN chmod ug+rwx $JBOSS_HOME/extensions/postconfigure.sh
RUN chmod -R ug+rwX $JBOSS_HOME
