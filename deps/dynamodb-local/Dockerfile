#
# Dockerfile for DynamoDB Local
#
# https://aws.amazon.com/blogs/aws/dynamodb-local-for-desktop-development/
#
FROM amazon/dynamodb-local:latest

# Create working space
WORKDIR /var/dynamodb_wd

# Default port for DynamoDB Local
EXPOSE 8000

# Add VOLUMEs to allow backup of config, logs and databases
VOLUME ["/var/dynamodb_local", "/var/dynamodb_wd"]
ENTRYPOINT ["sh"]
CMD ["-port", "8000"]
#CMD ["-jar", "DynamoDBLocal.jar", "-sharedDb", "-dbPath", "/var/dynamodb_local"]