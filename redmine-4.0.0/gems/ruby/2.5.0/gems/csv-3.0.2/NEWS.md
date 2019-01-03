# News

## 3.0.2 - 2018-12-23

### Improvements

  * Changed to use strscan in parser.
    [GitHub#52][Patch by 284km]

  * Improves CSV write performance.
    3.0.2 will be about 2 times faster than 3.0.1.

  * Improves CSV parse performance for complex case.
    3.0.2 will be about 2 times faster than 3.0.1.

### Fixes

  * Fixed a parse error bug for new line only input with `headers` option.
    [GitHub#53][Reported by Chris Beer]

  * Fixed some typos in document.
    [GitHub#54][Patch by Victor Shepelev]

### Thanks

  * 284km

  * Chris Beer

  * Victor Shepelev

## 3.0.1 - 2018-12-07

### Improvements

  * Added a test.
    [GitHub#38][Patch by 284km]

  * `CSV::Row#dup`: Changed to duplicate internal data.
    [GitHub#39][Reported by André Guimarães Sakata]

  * Documented `:nil_value` and `:empty_value` options.
    [GitHub#41][Patch by OwlWorks]

  * Added support for separator detection for non-seekable inputs.
    [GitHub#45][Patch by Ilmari Karonen]

  * Removed needless code.
    [GitHub#48][Patch by Espartaco Palma]

  * Added support for parsing header only CSV with `headers: true`.
    [GitHub#47][Patch by Kazuma Shibasaka]

  * Added support for coverage report in CI.
    [GitHub#48][Patch by Espartaco Palma]

  * Improved auto CR row separator detection.
    [GitHub#51][Reported by Yuki Kurihara]

### Fixes

  * Fixed a typo in document.
    [GitHub#40][Patch by Marcus Stollsteimer]

### Thanks

  * 284km

  * André Guimarães Sakata

  * Marcus Stollsteimer

  * OwlWorks

  * Ilmari Karonen

  * Espartaco Palma

  * Kazuma Shibasaka

  * Yuki Kurihara

## 3.0.0 - 2018-06-06

### Fixes

  * Fixed a bug that header isn't returned for empty row.
    [GitHub#37][Patch by Grace Lee]

### Thanks

  * Grace Lee

## 1.0.2 - 2018-05-03

### Improvements

  * Split file for CSV::VERSION

  * Code cleanup: Split csv.rb into a more manageable structure
    [GitHub#19][Patch by Espartaco Palma]
    [GitHub#20][Patch by Steven Daniels]

  * Use CSV::MalformedCSVError for invalid encoding line
    [GitHub#26][Reported by deepj]

  * Support implicit Row <-> Array conversion
    [Bug #10013][ruby-core:63582][Reported by Dawid Janczak]

  * Update class docs
    [GitHub#32][Patch by zverok]

  * Add `Row#each_pair`
    [GitHub#33][Patch by zverok]

  * Improve CSV performance
    [GitHub#30][Patch by Watson]

  * Add :nil_value and :empty_value option

### Fixes

  * Fix a bug that "bom|utf-8" doesn't work
    [GitHub#23][Reported by Pavel Lobashov]

  * `CSV::Row#to_h`, `#to_hash`: uses the same value as `Row#[]`
    [Bug #14482][Reported by tomoya ishida]

  * Make row separator detection more robust
    [GitHub#25][Reported by deepj]

  * Fix a bug that too much separator when col_sep is `" "`
    [Bug #8784][ruby-core:63582][Reported by Sylvain Laperche]

### Thanks

  * Espartaco Palma

  * Steven Daniels

  * deepj

  * Dawid Janczak

  * zverok

  * Watson

  * Pavel Lobashov

  * tomoya ishida

  * Sylvain Laperche

  * Ryunosuke Sato

## 1.0.1 - 2018-02-09

### Improvements

  * `CSV::Table#delete`: Added bulk delete support. You can delete
    multiple rows and columns at once.
    [GitHub#4][Patch by Vladislav]

  * Updated Gem description.
    [GitHub#11][Patch by Marcus Stollsteimer]

  * Code cleanup.
    [GitHub#12][Patch by Marcus Stollsteimer]
    [GitHub#14][Patch by Steven Daniels]
    [GitHub#18][Patch by takkanm]

  * `CSV::Table#dig`: Added.
    [GitHub#15][Patch by Tomohiro Ogoke]

  * `CSV::Row#dig`: Added.
    [GitHub#15][Patch by Tomohiro Ogoke]

  * Added ISO 8601 support to date time converter.
    [GitHub#16]

### Fixes

  * Fixed wrong `CSV::VERSION`.
    [GitHub#10][Reported by Marcus Stollsteimer]

  * `CSV.generate`: Fixed a regression bug that `String` argument is
    ignored.
    [GitHub#13][Patch by pavel]

### Thanks

  * Vladislav

  * Marcus Stollsteimer

  * Steven Daniels

  * takkanm

  * Tomohiro Ogoke

  * pavel
