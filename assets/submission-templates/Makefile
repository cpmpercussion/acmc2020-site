MD_FILES=acmc2020-paper-template.md acmc2020-performance-template.md acmc2020-workshop-template.md
DOCX_FILES=$(MD_FILES:.md=.docx)

all: $(DOCX_FILES)

%.docx: %.md
	pandoc $< -o $@

.PHONY: clean
clean:
	rm $(MD_FILES)
