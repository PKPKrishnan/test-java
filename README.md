# test-java


git init

-----------------------------------------------
git config --global user.name 'Shaumik'

git config --global user.email 'sd@gmail.com'

git config --global color.ui 'auto'
-----------------------------------------------

git add -A

git commit -m "My first commit"
-----------------------------------------------

git pull https://github.com/PKPKrishnan/test-java.git

(or)

(git remote add origin https://github.com/PKPKrishnan/test-java.git
 git push -u origin)
------------------------------------------------

git push
------------------------------------------------

## build.gradle (project common)

apply from: 'dependencies.gradle'
apply plugin: 'java'

sourceCompatibility = 1.5

    repositories {
        mavenCentral()
    }

    dependencies {
        compile libraries.slf4j
        testCompile group: 'junit', name: 'junit', version: '4.11'
    }
    
    
## dependencies.gradle

project.ext.libraries = [
        slf4j: 'org.slf4j:slf4j-api:1.7.24'

]
    
    
