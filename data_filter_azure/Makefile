build: env
	. env/bin/activate

env: env/bin/activate

env/bin/activate:
	test -d env || virtualenv env
	. env/bin/activate; pip install -Ur requirements.txt; pip install -e .
	touch env/bin/activate

clean:
	rm -fr env
	rm -fr *.egg-info
