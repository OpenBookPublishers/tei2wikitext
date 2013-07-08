tei2wikitext
============

Small TEI to MediaWiki wikitext converter based on an XSTL stylesheet with a small web interface.

Can also test by translating the MediaWiki output into HTML using local tools, as follows:
 java -jar (some base)/Saxon9.4/saxon9he.jar -s:(some TEI file) -xsl:tei2wikitext.xsl > tei2wikitext_test.mediawiki &&
  pandoc -f mediawiki -t html -o tei2wikitext_test.html tei2wikitext_test.mediawiki

NOTE
* Currently rely on HTML "pragma" to indicate intended charset.

TODO
* there are TODO items in the XSLT file.
* point to, or include, test data.
* dependency info and versions.
* build info?
