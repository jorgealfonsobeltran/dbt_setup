FROM amazonlinux
RUN yum install -y sudo
RUN yum install -y git
RUN yum install -y tar
RUN yum install -y python37
ENV PATH "$PATH:/root/.local/bin"
RUN curl -O https://bootstrap.pypa.io/get-pip.py
RUN python3 get-pip.py --user
RUN pip install dbt
COPY ./config/dbt_test.tar.gz /
RUN tar xzvf dbt_test.tar.gz
COPY ./config/profiles.yml /root/.dbt/