FROM quay.io/jdenise/pipeline-wildfly-server:729382b0c0ed949a5b32ba3dadfd5d8e
COPY --chown=jboss:root deployments/* $JBOSS_HOME/standalone/deployments
COPY --chown=jboss:root extensions $JBOSS_HOME/extensions
RUN chmod ug+rwx $JBOSS_HOME/extensions/postconfigure.sh
RUN chmod -R ug+rwX $JBOSS_HOME
