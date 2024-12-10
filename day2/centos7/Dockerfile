FROM centos:7

RUN sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-* && \
	sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-* && \
	yum repolist && \
	yum install vim httpd -y && \
	yum clean all

#ENTRYPOINT ["/bin/bash"]
#CMD ["tail", "-F", "/dev/null"]

ENTRYPOINT ["/usr/sbin/httpd"]

CMD ["-D", "FOREGROUND"]
