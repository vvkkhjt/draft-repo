FROM hub.digi-sky.com/base/nodejs:8.9.4
ENV PORT 8080
EXPOSE 8080

ADD . /data/webapps
RUN cd /data/webapps && yarn install && npm run build
EXPOSE 8080
RUN chmod 777 run.sh
WORKDIR /data/webapps

CMD ["/data/webapps/run.sh"]
