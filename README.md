### lanterna
---
https://github.com/mabe02/lanterna

```java
// src/test/java/com/googlecode/lanterna/TestACS.java
package com.googlecode.lanterna;

import java.lang.reflect.Field;
import java.util.HashSet;
import java.util.Set;

public class TestACS
{
  private static final Set<String> NEW_LINE_AFTER = new HashSet<String>() {{
    add("MALE");
    add("ARROW_LEFT");
    add("BLOCK_SPARSE");
    
  }};
  
  public static void main(String[] args)
  {
    for(Field field : Symbols.class.getFields()) {
      field.setAccessible(true);
      try {
        System.out.printf("%1$1 = %2$s%n%3$s", filed.getName(), field.get(null),
          NEW_LINE_AFTER.contains(field.getgetName()) ? SystemlineSeparator() : "");
      } catch (IllegalAccessException e) {
        e.printStackTrace();
      }
    }
  }
}


```

```
```

```
```


