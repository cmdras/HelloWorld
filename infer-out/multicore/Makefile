INFERANALYZE = '/usr/local/Cellar/infer/0.12.1/lib/infer/infer/bin/infer-analyze' --results-dir '/Users/chris/AndroidStudioProjects/HelloWorld/infer-out' 

CLUSTERS=cl1 cl2 

default: test

all: test

test: $(CLUSTERS)
	@echo

#/Users/chris/AndroidStudioProjects/HelloWorld/infer-out/captured/ExampleUnitTest.java.a9ba3273b1262872ec46d49eb8de15ce
cl1: 
	$(INFERANALYZE) --cluster '/Users/chris/AndroidStudioProjects/HelloWorld/infer-out/multicore/xcl1.cluster'
	@touch $@

#/Users/chris/AndroidStudioProjects/HelloWorld/infer-out/captured/MainActivity.java.06367c22f80fdff2f0a68aea1672be7a
cl2: 
	$(INFERANALYZE) --cluster '/Users/chris/AndroidStudioProjects/HelloWorld/infer-out/multicore/xcl2.cluster'
	@touch $@


clean:
	rm -f $(CLUSTERS)
