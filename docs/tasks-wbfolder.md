> Create a wbfolder.wbl file to be used in Dev Hub - Extension Editor.

**`wbfolder:tmp`**
* Creates a wbfolder.wbl file in  the `.tmp` directory.
* Options used:  
  * `wbfolder.enabled`- Whether the task is enabled or not, defaults to `true`.
  * `wbfolder.cwd` - Working directory, defaults to `./.tmp`.
  * `wbfolder.src` - Source mask, defaults to `./**/*.*`.
  * `wbfolder.dest` - wbfolder.wbl file destination, defaults to `./.tmp/wbfolder.wbl`.

Note: The `wbfolder.wbl` file is only necessary if you want to allow users to open your visualization extension in Qlik Dev Hub. 
`wbfolder.wbl` is NOT required and necessary to run your visualization extension in Qlik Sense.
