FROM yaoguais/lnmp:1.2.0

EXPOSE 3306 3307 6379 6380 80 443 9000 27017


ADD scripts /scripts
RUN chmod a+x /scripts/run-all-services
RUN chmod a+x /scripts/mysql/docker-entrypoint.sh
RUN chmod a+x /scripts/redis/docker-entrypoint.sh
RUN chmod a+x /scripts/mongodb/docker-entrypoint.sh

ENTRYPOINT ["/scripts/run-all-services"]

