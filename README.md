# cloudUploader CLI

A bash-based CLI tool that allows users to qucikly uplaod files to azure storage , providing a simple and seamless upload experience similar to popular storage services

Upload a file with the command:

cd {the script path}
clouduploder 2>&1 | tee output.txt

2>&1 = redirect stderr to stdout
tee = reads from the standard input and writes to both standard output and one or more files at the same time. 

setup() = install az cli and login your azure 

filecheck() = ask for your file path and name before checking your file exist or not
                   if not 
                         the script end


fileupload() = ask for your azure storage account and container, then upload the file to it

uploadOuputAndError() = upload the output file that is written error and standard outcome to azure storage 

print_storage_list() = print storage blob list to ensure what files are in the container



