FROM quay.io/jdenise/pipeline-wildfly-server:edd785f6b599aa5e0da513f6df1f2d77
COPY --chown=jboss:root deployments/* $JBOSS_HOME/standalone/deployments
COPY --chown=jboss:root extensions $JBOSS_HOME/extensions
RUN chmod ug+rwx $JBOSS_HOME/extensions/postconfigure.sh
RUN chmod -R ug+rwX $JBOSS_HOME
