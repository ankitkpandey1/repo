FROM rabbitmq:3.8

# Define environment variables.
ENV RABBITMQ_USER rabbit-user
ENV RABBITMQ_PASSWORD rabbit-password
ENV RABBITMQ_PID_FILE /var/lib/rabbitmq/mnesia/rabbitmq
ENV RABBITMQ_VHOST main-queue

ADD init.sh /init.sh
RUN chmod +x /init.sh
EXPOSE 5672
CMD ["./init.sh"]

