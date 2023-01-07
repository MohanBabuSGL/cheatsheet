#FROM flink:1.14.3-java11

FROM optimusacr.azurecr.io/optimus-flink:1.14.3-java11

USER root

COPY lib /opt/flink/lib
COPY logback-console.xml /opt/flink/conf

#ADD startcmd-job.sh /tmp/startcmd-job.sh
#ADD startcmd-task.sh /tmp/startcmd-task.sh

RUN cd /tmp;\
chown flink:flink /opt/flink/lib/*;\
chmod 755 /opt/flink/lib/*;
#ls -lrt;\
#chmod 750 startcmd-job.sh ;\
#chmod 750 startcmd-task.sh ;

#CMD ["/bin/bash"]
#CMD ["/opt/flink/bin/jobmanager.sh","start-foreground"]
