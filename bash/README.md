| Commands                 | In current directory |
| ------------------------ | -------------------- |
| ./                       | In current directory |
| bash -x <script_name>    | Debug mode           |
| shellcheck <script_name> |                      |

| Commands | Output | Description |
| --- | --- | --- |
| name=”DevOps” |  | Variable - no spaces |
| ${name} | DevOps | Access variable |

| Commands | Output | Description |
| --- | --- | --- |
| name=”World” |  | Variable |
| echo “Hello, ${name}” | Hello, World | Variable expanding |
| echo ‘Hello, ${name}’ | Hello, ${name} | Literal text string |

| Commands | Output | Description |
| --- | --- | --- |
| message=”Hello    World” |  | Variable |
| echo ${message} | Hello World | Spaces collapsed |
| echo “${message}” | Hello    World | Spaces preserved |

| Commands | Output | Description |
| --- | --- | --- |
| touch “my important file.txt”
file=”my important file.txt” |  | Create file
Variable |
| rm ${file} | Error | Tries deleting my, important, file.txt |
| rm “${file}” |  | Deletes single file |
