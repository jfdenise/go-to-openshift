FROM quay.io/jdenise/pipeline-wildfly-server:b3b5909c9efb34ec30bda3bca9022f0e
COPY --chown=jboss:root deployments/* $JBOSS_HOME/standalone/deployments
COPY --chown=jboss:root extensions $JBOSS_HOME/extensions
RUN chmod ug+rwx $JBOSS_HOME/extensions/postconfigure.sh
RUN chmod -R ug+rwX $JBOSS_HOME
