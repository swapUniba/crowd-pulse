crowd-pulse
===========

Reactive and Extensible Social Extraction and Analysis System.

-----------

This package contains just a `build.gradle` file that, when built, fetches all the available
`pulse` and `crowd-pulse` modules and puts them in the classpath in order to make their plugins
available for use.

## Install

Download and build the gradle script file that references all Crowd Pulse plugins.

```shell
sudo wget https://github.com/swapUniba/crowd-pulse/archive/master.tar.gz -O crowd-pulse.tar.gz
sudo mkdir crowd-pulse
sudo mkdir crowd-pulse/logs
sudo tar -xvzf crowd-pulse.tar.gz -C crowd-pulse --strip-components 1
sudo rm crowd-pulse.tar.gz
sudo ./crowd-pulse/gradlew installDist -p crowd-pulse/
```

## Configure

Copy all `.properties` files and external resources (dictionaries, lists, etc.) in the
`/crowd-pulse/build/install/crowd-pulse/lib` directory.

## Run

Call the main executable:

```shell
$ ./crowd-pulse/build/install/crowd-pulse/bin/crowd-pulse
```

## Available plugins

All plugins in the following modules are included (links to repositories):

* [`swapUniba/pulse-email-notify`](https://github.com/swapUniba/pulse-email-notify)
* [`swapUniba/crowd-pulse-social-twitter`](https://github.com/swapUniba/crowd-pulse-social-twitter)
* [`swapUniba/crowd-pulse-social-facebook`](https://github.com/swapUniba/crowd-pulse-social-facebook)
* [`swapUniba/crowd-pulse-data-java`](https://github.com/swapUniba/crowd-pulse-data-java)
* [`swapUniba/crowd-pulse-detect-language-optimaize`](https://github.com/swapUniba/crowd-pulse-detect-language-optimaize)
* [`swapUniba/crowd-pulse-fix-geo-profile-google-maps`](https://github.com/swapUniba/crowd-pulse-fix-geo-profile-google-maps)
* [`swapUniba/crowd-pulse-fix-geo-message-from-profile`](https://github.com/swapUniba/crowd-pulse-fix-geo-message-from-profile)
* [`swapUniba/crowd-pulse-index-uniba`](https://github.com/swapUniba/crowd-pulse-index-uniba)
* [`swapUniba/crowd-pulse-tag-babelfy`](https://github.com/swapUniba/crowd-pulse-tag-babelfy)
* [`swapUniba/crowd-pulse-tag-me`](https://github.com/swapUniba/crowd-pulse-tag-me)
* [`swapUniba/crowd-pulse-tag-open-calais`](https://github.com/swapUniba/crowd-pulse-tag-open-calais)
* [`swapUniba/crowd-pulse-tag-wikipedia-miner`](https://github.com/swapUniba/crowd-pulse-tag-wikipedia-miner)
* [`swapUniba/crowd-pulse-categorize-wikipedia`](https://github.com/swapUniba/crowd-pulse-categorize-wikipedia)
* [`swapUniba/crowd-pulse-tokenize-open-nlp`](https://github.com/swapUniba/crowd-pulse-tokenize-open-nlp)
* [`swapUniba/crowd-pulse-lemmatize-morphit`](https://github.com/swapUniba/crowd-pulse-lemmatize-morphit)
* [`swapUniba/crowd-pulse-lemmatize-stanford-corenlp`](https://github.com/swapUniba/crowd-pulse-lemmatize-stanford-corenlp)
* [`swapUniba/crowd-pulse-pos-tag-open-nlp`](https://github.com/swapUniba/crowd-pulse-pos-tag-open-nlp)
* [`swapUniba/crowd-pulse-pos-tag-simple-it`](https://github.com/swapUniba/crowd-pulse-pos-tag-simple-it)
* [`swapUniba/crowd-pulse-pos-tag-simple-en`](https://github.com/swapUniba/crowd-pulse-pos-tag-simple-en)
* [`swapUniba/crowd-pulse-rem-stop-word-simple`](https://github.com/swapUniba/crowd-pulse-rem-stop-word-simple)
* [`swapUniba/crowd-pulse-sentiment-sentiwordnet`](https://github.com/swapUniba/crowd-pulse-sentiment-sentiwordnet)
* [`swapUniba/crowd-pulse-sentiment-meaningcloud`](https://github.com/swapUniba/crowd-pulse-sentiment-meaningcloud)
* [`swapUniba/crowd-pulse-jgibblda-estimator`](https://github.com/swapUniba/crowd-pulse-jgibblda-estimator)
* [`swapUniba/crowd-pulse-jgibblda-inferencer`](https://github.com/swapUniba/crowd-pulse-jgibblda-inferencer)
* [`swapUniba/crowd-pulse-app-categorize`](https://github.com/swapUniba/crowd-pulse-app-categorize)
* [`swapUniba/crowd-pulse-entity-labeller`](https://github.com/swapUniba/crowd-pulse-entity-labeller)
* [`swapUniba/crowd-pulse-machine-learning-training`](https://github.com/swapUniba/crowd-pulse-machine-learning-training)
* [`swapUniba/crowd-pulse-machine-learning-testing`](https://github.com/swapUniba/crowd-pulse-machine-learning-testing)

