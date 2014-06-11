Chat application
================

Red5 WebSocket chat application example.

The example <i>index.html</i> defaults to using a WebSocket connection to localhost on port 8081. This means that the localhost and port must be configured in the <i>red5/conf/jee-container.xml</i> file.

```xml
<bean id="webSocketTransport" class="org.red5.net.websocket.WebSocketTransport">
    <property name="addresses">
        <list>
            <value>localhost:8081</value>
        </list>
    </property>
</bean>
```

Build the application from the command line with

```bash
mvn package
```

Deploy your application by copying the war file into your <i>red5/webapps</i> directory.
