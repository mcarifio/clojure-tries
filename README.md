clojure-tries
=============

Exercises and examples from clojure books.

Setup
=====

* Installed clojure into /opt/clojure/clojure-${version}:

  <pre><code>
  sudo install -o $USERNAME -g $USERNAME -d /opt/clojure ## create a global /opt/clojure owned by you for convenience
  export clojure_version=1.5.1 ## or your version
  cd /opt/clojure; curl http://repo1.maven.org/maven2/org/clojure/clojure/${clojure_version}/clojure-${clojure_version}.zip | unzip - ## download and unzip, assume the zip is at the url
  ln -s clojure-${clojure_version} current
  echo 'export CLOJURE_ROOT=/opt/clojure/current' | sudo tee /etc/profile.d/clojure.sh
  source /etc/profile.d/clojure.sh
  </code></pre>  

* Install [Leiningrad] (https://github.com/technomancy/leiningen):

  <pre><code>
  mkdir $CLOJURE_ROOT/bin; cd $CLOJURE_ROOT/bin
  wget https://raw.github.com/technomancy/leiningen/stable/bin/lein
  chmod a+x lein
  export PATH=$CLOJURE_ROOT/bin:$PATH
  lein version ## jar installe in ~/.lein/self-install
  Leiningen 2.3.2 on Java 1.8.0-ea Java HotSpot(TM) 64-Bit Server VM
  </pre></code>


TODO
====

* Better way to handle code fragments in Markdown?

* Using git for ticket management?


