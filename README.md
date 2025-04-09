
# West Manifest Repo For Knowledge Library

## Usage: Workspace Initialization

To initialize a T2 topology workspace using the west.yml manifest provided by this repository.

1. use `west init` to create the workspace

   ```console
   
   west init -m https://github.com/richMetellus/doc_manifest_repo \
   --mr main \
   <path/to/workspace>
   ```

   - `west init -m` to specify another manifest repository since by default west would look at zephyr.
   - `--mr` to use a revision to initialize from
   - `<path/to/workspace>` replace this to the desired workspace you want west to initialized the project in.

2. then update the projects in the workspace.

   ```console
   cd <path/to/workspace>
   west update 
   ```

   **Note**: you can use `west topdir` command to print the top level directory
   of the workspace.
