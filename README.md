# .-Write-a-Python-program-to-write-a-list-to-a-file.
def write_list_to_file(file_path, data_list):
    try:
        with open(file_path, 'w') as file:
            for item in data_list:
                file.write(str(item) + '\n')
        print("List written to the file successfully.")
    except IOError:
        print("An error occurred while writing to the file.")

# Example usage
file_path = 'path/to/your/file.txt'  # Replace with the actual file path
data_list = [1, 2, 3, 4, 5]
write_list_to_file(file_path, data_list)
