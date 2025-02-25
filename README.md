
# How to run sdkbox samples

Steps:

~~~bash
mkdir samples
cd samples

# must clone this repo
git clone --depth 1 https://github.com/sdkbox/sdkbox-cocos2d-x-binary.git

# clone sample repo
git clone --depth 1 https://github.com/sdkbox/sdkbox-sample-ga.git

# run sample with specified language and platform
# eg: cpp and ios
./sdkbox-cocos2d-x-binary/run_sample.sh ga cpp ios
## or
cd cpp && cocos run -p ios

# javascript and android
./sdkbox-cocos2d-x-binary/run_sample.sh ga js android
## or
cd js && cocos run -p android

# <optional> if exists "download-depends.sh" in sample repo, execute it
# ./sdkbox-sample-ga/download-depends.sh

~~~

Memo:

1.  Sample repo and cocos2dx repo must be in same level directory

~~~
+-- sdkbox-cocos2d-x-binary
+-- sdkbox-sample-ga
| +-- cpp
| +-- lua
| \-- js
~~~
