cq5-basic
=========

a basic structure for adobe cq5 maven projects

maven commands:

1) install only bundles to cq5

mvn -Pbundles,cq-install clean install


2) install only content to cq5

mvn -Pcontent,cq-install clean install


3) install entire application to cq5 as single CRX package

mvn -Pbundles,content,release,release-install clean install