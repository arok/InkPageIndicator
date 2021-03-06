# InkPageIndicator
InkPageIndicator from Plaid https://github.com/nickbutcher/plaid. Works with API 19+ (4.4+)

![Sample Gif](http://fat.gfycat.com/JitteryGenuineFugu.gif)

[![Build Status](https://travis-ci.org/Commit451/InkPageIndicator.svg?branch=master)](https://travis-ci.org/Commit451/InkPageIndicator)

# Gradle Dependency
Easily reference the library in your Android projects using this dependency in your module's `build.gradle` file:

```Gradle
dependencies {
    compile 'com.commit451:inkpageindicator:1.0.2'
}
```

# Usage
See the sample app for a full example. Basic usage:

```xml
<com.commit451.inkpageindicator.InkPageIndicator
  android:id="@+id/ink_pager_indicator"
  android:layout_width="match_parent"
  android:layout_height="wrap_content"/>
```

```java
InkPageIndicator inkPageIndicator = (InkPageIndicator) findViewById(R.id.ink_pager_indicator);
inkPageIndicator.setViewPager(viewPager);
```

# Custom Attributes
The library also supports styling in XML:
```xml
<com.commit451.inkpageindicator.InkPageIndicator
  android:id="@+id/ink_pager_indicator"
  android:layout_width="match_parent"
  android:layout_height="wrap_content"
  app:dotDiameter="4dp"
  app:dotGap="4dp"
  app:animationDuration="200"
  app:pageIndicatorColor="@color/orange"
  app:currentPageIndicatorColor="@color/white"/>
```

# Contributions
Please make pull requests as you see fit and log issues so that others can benefit from knowing the library and its issues. 

Special thanks to @nickbutcher for the original code and @hzsweers for backporting it to 4.4+

License
--------

    Copyright 2015 Google Inc., Commit 451

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
