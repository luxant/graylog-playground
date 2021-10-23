# Sending logs by http to graylog
- Configure a Gelf Http input on graylog
- Then:

```
curl -X POST -H "Content-Type: application/json" -d '{"version": "1.1", "host": "myhost", "short_message": "Hello World!", "full_message": "Hello World!"} 'http://graylog:12201/gelf'
```


# References:

## Graylog forum

https://community.graylog.org/t/send-log-data-by-api-in-graylog/5978

## Graylog docs

https://archivedocs.graylog.org/en/2.4/pages/gelf.html#sending-gelf-messages-via-http-using-curl

## Graylog repo

https://github.com/Graylog2/docker-compose