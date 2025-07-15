for room database add in project

//room plugins in two build gradle 

at first - in project(not module app): in plugin ---  id("com.google.devtools.ksp") version "2.0.21-1.0.27" apply false
then - in build gradle (module app): in plugin --- id("com.google.devtools.ksp")

in dependencies ---- // Room version
def room_version = "2.6.1"

// Room dependencies with KSP
implementation "androidx.room:room-runtime:$room_version"
implementation "androidx.room:room-ktx:$room_version"
ksp "androidx.room:room-compiler:$room_version"
