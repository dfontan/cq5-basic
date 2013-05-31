cq5-basic
=========

a basic structure for adobe cq5 maven projects

maven commands:

1) install only bundles to cq5

<project-root>/mvn -Pbundles,cq-install
						[-Dtarget.url=<your running cq5 instance, if not localhost:4502>]
						[-Dcrx.user=<crx user, if not admin>]
						[-Dcrx.password=<crx password, if not admin>]
						[clean]
					install


2) install only content to cq5

<project-root>/mvn -Pcontent,cq-install
						[-Dtarget.url=<your running cq5 instance, if not localhost:4502>]
						[-Dcrx.user=<crx user, if not admin>]
						[-Dcrx.password=<crx password, if not admin>]
						[clean]
					install


3) install entire application to cq5 as single CRX package

<project-root>/mvn -Pbundles,content,release,release-install
						[-Dtarget.url=<your running cq5 instance, if not localhost:4502>]
						[-Dcrx.user=<crx user, if not admin>]
						[-Dcrx.password=<crx password, if not admin>]
						[clean]
					install


4) install specific module to cq5

<project-root>/<module>/mvn -Pcq-install
						[-Dtarget.url=<your running cq5 instance, if not localhost:4502>]
						[-Dcrx.user=<crx user, if not admin>]
						[-Dcrx.password=<crx password, if not admin>]
						[clean]
					install
