# Dockerfile for Hadoop namenode.

FROM hal433/hadoop-base

ENV HDFS_CONF_dfs_namenode_name_dir=file:///hadoop/dfs/name
RUN mkdir -p /hadoop/dfs/name
VOLUME /hadoop/dfs/name

COPY files/namenode-run.sh /entrypoints/namenode-run.sh
RUN chmod a+x /entrypoints/namenode-run.sh

CMD ["/entrypoints/namenode-run.sh"]
