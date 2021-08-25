# Protocol Buffer

- Install Protoc Compiler
    - The source code representing the given proto files can be automatically generated in different programming languages using the protoc tool via the command line.
    - Download **protoc-3.17.3-win64.zip** from https://github.com/protocolbuffers/protobuf/releases for windows.

- Commands
    -  Command to Generate **Java** Files
        ```bash
        protoc -I=<path_to_proto_files_directory> --java_out=<directory_path_for_genereated_java_files> <path_to_proto_files_directory>/*.proto 
        ```
        - Example: (To be run from the root directory of the git repository)
            - Generating **Java** Files:
                ```bash
                protoc -I=protocol-buffers/1_example --java_out=protocol-buffers/java/1_example protocol-buffers/1_example/*.proto
                ```
            -  Generating **Python** Files:
                ```bash
                protoc -I=protocol-buffers/1_example --python_out=protocol-buffers/python/1_example protocol-buffers/1_example/*.proto
                ```
            - Generating **JavaScript** Files:
                ```bash
                protoc -I=protocol-buffers/1_example --js_out=protocol-buffers/javascript/1_example protocol-buffers/1_example/*.proto
                ```

        
