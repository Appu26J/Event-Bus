# Event Bus
A very simple and fast event bus in Java!  
*(There's no library for this as the code is just 2 classes so you can just drag it to your project)*

### Example Usage
```java
private EventBus bus = new EventBus();

public void init()
{
    bus.register(this);
}

public void onSomeEvent()
{
    bus.post(new ExampleEvent());
}

@Subscribe
public void onExampleEvent(ExampleEvent e)
{
    System.out.println("event has been called!");
}
```
