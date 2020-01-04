# Zoom Recyler Layout

[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)
[![API](https://img.shields.io/badge/API-11%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=22)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0.html)

Beautiful RecyclerView Zoom Animation for Android

## Preview
![gif](https://raw.githubusercontent.com/Spikeysanju/ZoomRecylerLayout/master/ezgif.com-video-to-gif.gif)

## About

Refer Here [Wiki](https://github.com/yadav-rahul/TastyToast/wiki)

## Dependency

Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:



```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

```

## Dependency

Add dependency in your app module

```
	dependencies {
	        implementation 'com.github.Spikeysanju:ZoomRecylerLayout:1.0'
	}

```

## Usage

### Kotlin
```
        val linearLayoutManager = ZoomRecylerLayout(this)
```

### Detailed Usage
```

        val linearLayoutManager = CenterZoomLayoutManager(this)
        linearLayoutManager.orientation = LinearLayoutManager.HORIZONTAL
        linearLayoutManager.reverseLayout = true
        linearLayoutManager.stackFromEnd = true
        toursRV.layoutManager = linearLayoutManager
```
### Orientation Types
```

        linearLayoutManager.orientation = LinearLayoutManager.HORIZONTAL
        linearLayoutManager.orientation = LinearLayoutManager.VERTICAL

        
```

### Use SnapHelper for Auto Center Views
```
        val snapHelper = LinearSnapHelper()
        snapHelper.attachToRecyclerView(toursRV)
        toursRV.isNestedScrollingEnabled = false
```


Last parameter here is the type of toast you want to show.

## Contributing

Please fork this repository and contribute back using
[pull requests](https://github.com/Spikeysanju/ZoomRecylerLayout/pulls).

Any contributions, large or small, major features, bug fixes, are welcomed and appreciated
but will be thoroughly reviewed .

## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

```
Copyright 2016 Spikey Sanju

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
