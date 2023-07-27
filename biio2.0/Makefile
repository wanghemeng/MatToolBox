.PHONY: compile analysis convert clean

data_path="/home/hemeng/Documents/Data/matrices/"

compile:
	gcc ./src/convert.c -o ./bin/convert

analysis:
	gcc ./src/analysis.c -o ./bin/analysis

convert:
	@for data in `find $(data_path) -name "*.mtx"`; \
	do \
		./bin/convert $$data; \
	done

clean:
	rm ./bin/*