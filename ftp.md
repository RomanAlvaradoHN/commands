# Using the scp command
The `scp` command can be used to transfer files between machines over a secure, encrypted connection.  

### General Sintax
`scp [options] [localfile's] username@hostname:[remotefile]`

### Options
| Option   | Meaning                                                                |
| :------  | :------                                                                |
| `-r`     | Recursively copy entire directories.                                   |
| `-P`     | Specify the port to connect to on the remote host (It is a capital P). |
| `-i`     | Specify an identity private key file.                                  |
| `-C`     | Enable compression.                                                    |
| `-v`     | Enable verbose mode.                                                   |
| `-l`     | Limit the bandwidth used by the copy.                                  |



# Using the sftp command

### General Sintax
`sftp username@hostname` - This command will create a new session ("sftp>" promt).
`[option] [operation] [file's]` - This command is used to transfer files.

### Options
| Command  | Meaning                                            |
| :------  | :------                                            |
| `-P`     | Specify the port to connect to on the remote host. |
| `-i`     | Specify an identity private key file.              |
| `-r`     | Recursively copy entire directories.               |

### Operations
| Operation  | Meaning                                          |
| :------    | :------                                          |
| `get`      | Download a file                                  |
| `put`      | Upload a file                                    |
| `ls`       | List the current remote directory                |
| `lls`      | List the current local directory                 |
| `pwd`      | Show the current remote directory                |
| `lpwd`     | Show the current local directory                 |
| `cd`       | Change remote directory                          |
| `lcd`      | Change local directory                           |
| `exit`     | Ends session                                     |