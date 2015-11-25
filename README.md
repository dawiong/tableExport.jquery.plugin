tableExport.jquery.plugin
=========================

Original plugin from https://github.com/hhurz/tableExport.jquery.plugin . Work in progress and so the main tableExport.js is only changed so far (no minifications, testing, etc.).

Just sharing, for people experiencing the same problem that the download does not work in IE (data-uri not supported in IE), solution from sampopes' answer on http://stackoverflow.com/questions/22317951/export-html-table-data-to-excel-using-javascript-jquery-is-not-working-properl .

NOTE: My changes are not elegant, it's patchy since I only need it for my use case (XLS), so just giving an idea on how this may work.

1. XLS only, I might decide to rework it for everything if I have time.
2. Added regexp for <select> since if there are filter control dropdowns, I do not want to include the options in the header.
3. This is not a permanent solution since IE may handle the iframe workaround differently in the future.
