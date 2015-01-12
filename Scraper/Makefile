module: Scraper.swiftmodule Scraper.a
	
Scraper.swiftmodule:
	xcrun -sdk macosx swiftc -emit-module Scraper.swift -module-name Scraper

Scraper.a: Scraper.o
	ar rcs libScraper.a Scraper.o

Scraper.o:
	xcrun -sdk macosx swiftc -emit-library -emit-object Scraper.swift -module-name Scraper

clean:
	rm -f Scraper.o Scraper.swiftdoc Scraper.swiftmodule libScraper.a

