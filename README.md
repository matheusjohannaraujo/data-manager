
# DataManager

**DataManager** is a PHP library developed to simplify file and directory manipulation, offering an intuitive class for common filesystem operations.

## 📦 Installation

You can install the library via [Packagist/Composer](https://packagist.org/packages/mjohann/data-manager):

```bash
composer require mjohann/data-manager
```

## ⚙️ Requirements

- PHP 7.0 or higher

## 🚀 Features

- Create, read, update, and delete files  
- Create and delete directories  
- List files and directories  
- Check for the existence of files or directories  
- Read and write content to files  
- Rename files and directories  
- Get detailed information about files

## 🧪 Usage Example

```php
<?php
require_once "vendor/autoload.php";

use MJohann\Packlib\DataManager;

// Create a new folder named "my_dir"
DataManager::folderCreate("my_dir");

// Create a new file "file.txt" inside "my_dir" and write "Test DataManager" to it
DataManager::fileCreate("my_dir/file.txt", "Test DataManager");

// Read the contents of "my_dir/file.txt" and print it
echo DataManager::fileRead("my_dir/file.txt"), PHP_EOL;

// Get and print the size of the "my_dir" folder
echo DataManager::size("my_dir/"), PHP_EOL;

// Scan the "my_dir" folder and print its contents as an array
var_export(DataManager::folderScan("my_dir/"));
```

For more examples, see the [`example/script.php`](example/script.php) file in the repository.

## 📁 Project Structure

```
data-manager/
├── src/
│   └── DataManager.php
├── example/
│   └── script.php
├── composer.json
├── .gitignore
├── LICENSE
└── README.md
```

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## 👨‍💻 Author

Developed by [Matheus Johann Araújo](https://github.com/matheusjohannaraujo) – Pernambuco, Brazil.
