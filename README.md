# Useful switches

--verbose: Prints out verbose logging to explain what is going on (may be combined with any other flag)
--dry: Shows what would be done but does not actually build anything
--clean: Deletes the outputs of the specified projects (may be combined with --dry)
--force: Acts as if all projects are out of date
--watch: Watch mode (may not be combined with any flag except --verbose)

# key points in tsconfig.json

"composite": true instructs tsc that there are project references
"declarationMap": true adds source maps for .d.ts declaration files. It means Go to Definition in VS code and will go to the actual file and not the .d.ts file
The paths field contains an object with each object key (common, web, or API in this example) pointing to a package’s location. With this set, we can import packages without a nasty relative or absolute path.
e.g. import { a } from 'web';
