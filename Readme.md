# Widgets

Android Material Design widgets for Android 9+

### 1. Floating Edit Text
![alt text](https://github.com/manupsunny/Widgets/blob/master/resources/FloatingEditText.gif "FloatingEditText")

#### Dependency

Soon to be uploaded to Maven

#### Usage
```
<com.manusunny.android.FloatingEditText
        android:id="@+id/floatingEditText"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Floating Edit Text"
        android:textColor="@android:color/black"
        app:hint_scale="0.5"
        app:hint_color="@color/colorPrimary"
        app:highlighted_color="@color/colorAccent"
        app:error_color="@color/colorError"
        app:underline_height="1dp"
        app:underline_highlighted_height="2dp"/>
```

To set error indication:

```
FloatingEditText editText = (FloatingEditText) findViewById(R.id.floatingEditText);
editText.setValidationResult(false, "Invalid Input");
```

Other available methods : 

```
editText.setHighlightedColor(highlightedColor);
editText.setNormalColor(normalColor);
editText.setErrorColor(errorColor);
```
#### Styling

Give required styles in `res/values/styles.xml`

Example:
```xml
<resources>
    <style name="FloatingEditText" >
        <item name="hint_scale">0.5</item>
        <item name="hint_color">@color/colorPrimary</item>
        <item name="highlighted_color">@color/colorAccent</item>
        <item name="error_color">#FFFFFF</item>
        
        <item name="underline_height">8dp</item>
        <item name="underline_highlighted_height">200dp</item>
    </style>
</resources>
```
## License

    Copyright 2015 © Manu Sunny

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
