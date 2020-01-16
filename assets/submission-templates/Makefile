MD_FILES=acmc2020-paper-template.md acmc2020-performance-template.md acmc2020-workshop-template.md
DOCX_FILES=$(MD_FILES:.md=.docx)
ODT_FILES=$(MD_FILES:.md=.odt)

all: $(DOCX_FILES) $(ODT_FILES)

%.docx: %.md
	pandoc $< -o $@

%.odt: %.md
	pandoc $< -o $@

.PHONY: clean
clean:
	rm $(MD_FILES)
