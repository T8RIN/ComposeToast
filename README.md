# ComposeToast
Animated Jetpack Compose replacement of android standard Toast messages

```kotlin
//Usage example
val toastHostState = remember { ToastHostState() }
val scope = rememberCoroutineScope()

Button(
    onClick = { 
        scope.launch {
            toastHostState.showToast(/*Your Visuals*/)
        }
    }
) {
    Text("Show Toast")
}

ToastHost(hostState = toastHostState)
```

## Note 
Also remember to add this dependencies to local build.gradle folder
```kotlin
implementation("org.jetbrains.kotlinx:kotlinx-coroutines-core:1.6.4")
implementation("androidx.compose.ui:ui:1.4.0-alpha03")
implementation("androidx.compose.material3:material3:1.1.0-alpha03")
```

## Find this repository useful? :heart:
Support it by joining __[stargazers](https://github.com/t8rin/marquee/stargazers)__ for this repository. :star: <br>
And __[follow](https://github.com/t8rin)__ me for my next creations! 🤩

# License
```xml
Designed and developed by 2023 T8RIN

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
