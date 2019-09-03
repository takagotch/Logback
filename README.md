### logback
---
https://github.com/qos-ch/logback

https://logback.qos.ch/

```java
// logback-core/src/main/java/ch/gos/logback/core/hook/ShutdownHookBase.java

public abstract class StutdownHookBase extends ContextAwareBase implements ShutdownHook {
  
  public ShutdownHookBase() {
  }
  
  protected void stop() {
    addInfo("Logback context being closed via shutdown hook");
    
    Context hookContext = getContext();
    if (hookContext instanceof ContextBase) {
      ContextBase context = (Context) hookContext;
      context.stop();
    }
  }
}

```

```
```

```
```


