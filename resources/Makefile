QOOXDOO_PATH = ../../../..
SPHINX_THEME = _theme.indigo

css: scss/*.scss
	scss -t expanded --sourcemap=none scss/base.scss stylesheets/base.css
	scss -t expanded --sourcemap=none scss/layout.scss stylesheets/layout.css
	scss -t expanded --sourcemap=none scss/pages.scss stylesheets/pages.css
	scss -t expanded --sourcemap=none scss/reset.scss stylesheets/reset.css

# the next is more of a note, to keep things in mind
manual: css
	@cp -R fonts $(QOOXDOO_PATH)/documentation/manual/source/$(SPHINX_THEME)
	@cp stylesheets/* $(QOOXDOO_PATH)/documentation/manual/source/$(SPHINX_THEME)/copies
	@cp javascripts/* $(QOOXDOO_PATH)/documentation/manual/source/$(SPHINX_THEME)/copies
