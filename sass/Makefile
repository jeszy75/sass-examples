sources = $(wildcard *.scss)
targets = $(sources:.scss=.css)

SASS = sass
SASS_FLAGS =

.PHONY: all
all: $(targets)

%.css: %.scss
	$(SASS) $< $@ $(SASS_FLAGS)

.PHONY: clean
clean:
	rm -f $(targets) $(targets:.css=.css.map)
